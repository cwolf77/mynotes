# To Consider

## Schema definition

Each example launches Solr with a managed schema, which allows use of the [Schema API](http://lucene.apache.org/solr/guide/7_2/schema-api.html#schema-api) to make schema edits, but does not allow manual editing of a Schema file.

If you would prefer to manually modify a`schema.xml`file directly, you can change this default as described in the section [Schema Factory Definition in SolrConfig](http://lucene.apache.org/solr/guide/7_2/schema-factory-definition-in-solrconfig.html#schema-factory-definition-in-solrconfig).

## Facet
If you want Solr to perform both analysis (for searching) and faceting on the full literal strings, use the copyField directive in your Schema to create two versions of the field: one Text and one String. Make sure both are indexed="true". (For more information about the copyField directive, see Documents, Fields, and Schema Design.)

## Tika

In the available examples there is a Tika DIH \(DataImporterHandler\). It would be nice to check how it works. Maybe we can use it somehow for fulltext search.

