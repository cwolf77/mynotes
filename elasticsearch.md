# ElasticSearch

## About official clients API

[https://www.elastic.co/guide/en/elasticsearch/client/index.html](https://www.elastic.co/guide/en/elasticsearch/client/index.html "Elasticsearch Clients")

[https://www.elastic.co/blog/found-interfacing-elasticsearch-picking-client](https://www.elastic.co/blog/found-interfacing-elasticsearch-picking-client "Interfacing with Elasticsearch: Picking a Client")

[https://www.elastic.co/blog/benchmarking-rest-client-transport-client](https://www.elastic.co/blog/benchmarking-rest-client-transport-client "Benchmarking REST client and transport client")

[https://www.elastic.co/blog/state-of-the-official-elasticsearch-java-clients](https://www.elastic.co/blog/state-of-the-official-elasticsearch-java-clients "State of the official Elasticsearch Java clients")

[https://www.javacodegeeks.com/2017/03/elasticsearch-java-developers-elasticsearch-java.html](https://www.javacodegeeks.com/2017/03/elasticsearch-java-developers-elasticsearch-java.html)

## Alternate non ElasticSearch official clients

### Jest client

When writting those lines, Jest seems to support only ES version 2.X.

[https://github.com/searchbox-io/Jest/tree/master/jest](https://github.com/searchbox-io/Jest/tree/master/jest)

## Indexing binary file

[https://stackoverflow.com/questions/34857179/how-to-index-a-pdf-file-in-elasticsearch](https://stackoverflow.com/questions/34857179/how-to-index-a-pdf-file-in-elasticsearch)

[https://ambar.cloud/](https://ambar.cloud/)

[https://stackoverflow.com/questions/37861279/how-to-index-a-pdf-file-in-elasticsearch-5-0-0-with-ingest-attachment-plugin?rq=1](https://stackoverflow.com/questions/37861279/how-to-index-a-pdf-file-in-elasticsearch-5-0-0-with-ingest-attachment-plugin?rq=1)

[https://stackoverflow.com/questions/42109961/how-to-index-a-pdf-file-using-elasticsearch-ingest-attachment-plugin](https://stackoverflow.com/questions/42109961/how-to-index-a-pdf-file-using-elasticsearch-ingest-attachment-plugin)

[https://blog.ambar.cloud/ingesting-documents-pdf-word-txt-etc-into-elasticsearch/](https://blog.ambar.cloud/ingesting-documents-pdf-word-txt-etc-into-elasticsearch/)

[https://www.quora.com/How-can-Elasticsearch-be-used-for-indexing-the-full-text-of-PDF-and-Microsoft-Office-documents](https://www.quora.com/How-can-Elasticsearch-be-used-for-indexing-the-full-text-of-PDF-and-Microsoft-Office-documents)

[https://www.opensemanticsearch.org/connector/files/pdf](https://www.opensemanticsearch.org/connector/files/pdf)

[https://qbox.io/blog/index-attachments-files-elasticsearch-mapper](https://qbox.io/blog/index-attachments-files-elasticsearch-mapper)

## Index

### Organize index

[https://blog.ambar.cloud/ambar-use-case-integrated-parse-and-search-solution/](https://blog.ambar.cloud/ambar-use-case-integrated-parse-and-search-solution/)

### Full Text

[https://www.elastic.co/guide/en/elasticsearch/reference/current/text.html](https://www.elastic.co/guide/en/elasticsearch/reference/current/text.html)

### Performance with large text index

[https://blog.ambar.cloud/making-elasticsearch-perform-well-with-large-text-fields/](https://blog.ambar.cloud/making-elasticsearch-perform-well-with-large-text-fields/)

### Meta-Files \(\_routing, \_meta, ...\)

[https://www.elastic.co/guide/en/elasticsearch/reference/current/mapping-fields.html](https://www.elastic.co/guide/en/elasticsearch/reference/current/mapping-fields.html)

### Mapping \(field datatypes, dynamic mapping, dynamic templates,...\)

[https://www.elastic.co/guide/en/elasticsearch/reference/current/mapping.html](https://www.elastic.co/guide/en/elasticsearch/reference/current/mapping.html)

## Search

[https://www.elastic.co/guide/en/elasticsearch/reference/current/how-to.html](https://www.elastic.co/guide/en/elasticsearch/reference/current/how-to.html)

[https://www.elastic.co/guide/en/elasticsearch/reference/current/tune-for-disk-usage.html](https://www.elastic.co/guide/en/elasticsearch/reference/current/tune-for-disk-usage.html)

### Improve search on string

[https://www.elastic.co/guide/en/elasticsearch/reference/current/tune-for-disk-usage.html\\#\\_don\\_8217\\_t\\_use\\_default\\_dynamic\\_string\\_mappings](https://www.elastic.co/guide/en/elasticsearch/reference/current/tune-for-disk-usage.html\#\_don\_8217\_t\_use\_default\_dynamic\_string\_mappings)

## Test

**Maven plugin** : [https://github.com/alexcojocaru/elasticsearch-maven-plugin/tree/es5](https://github.com/alexcojocaru/elasticsearch-maven-plugin/tree/es5)

Reason why not using ESIntegTestCase : https://discuss.elastic.co/t/5-0-0-using-painless-in-esintegtestcase/64447/14

