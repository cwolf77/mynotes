# To Consider

## Schema definition

Each example launches Solr with a managed schema, which allows use of the [Schema API](http://lucene.apache.org/solr/guide/7_2/schema-api.html#schema-api) to make schema edits, but does not allow manual editing of a Schema file.

If you would prefer to manually modify a`schema.xml`file directly, you can change this default as described in the section [Schema Factory Definition in SolrConfig](http://lucene.apache.org/solr/guide/7_2/schema-factory-definition-in-solrconfig.html#schema-factory-definition-in-solrconfig).

## Facet

### Faceting on full literal strings
If you want Solr to perform both analysis (for searching) and faceting on the full literal strings, use the copyField directive in your Schema to create two versions of the field: one Text and one String. Make sure both are indexed="true". (For more information about the copyField directive, see Documents, Fields, and Schema Design.)

### Local Parameters for Faceting
The LocalParams syntax allows overriding global settings. It can also provide a method of adding metadata to other parameter values, much like XML attributes.

Tagging and Excluding Filters
You can tag specific filters and exclude those filters when faceting. This is useful when doing multi-select faceting.

Consider the following example query with faceting:

`q=mainquery&fq=status:public&fq=doctype:pdf&facet=true&facet.field=doctype`

Because everything is already constrained by the filter doctype:pdf, the facet.field=doctype facet command is currently redundant and will return 0 counts for everything except doctype:pdf.

To implement a multi-select facet for doctype, a GUI may want to still display the other doctype values and their associated counts, as if the doctype:pdf constraint had not yet been applied. For example:


`\[ \] Word (42)`


To return counts for doctype values that are currently not selected, tag filters that directly constrain doctype, and exclude those filters when faceting on doctype.

`q=mainquery&fq=status:public&fq={!tag=dt}doctype:pdf&facet=true&facet.field={!ex=dt}doctype`

Filter exclusion is supported for all types of facets. Both the tag and ex local parameters may specify multiple values by separating them with commas.

## Tika

In the available examples there is a Tika DIH \(DataImporterHandler\). It would be nice to check how it works. Maybe we can use it somehow for fulltext search.

