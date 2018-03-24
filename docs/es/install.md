# 环境安装

## [Mac]安装ElasticSearch

下载地址：https://www.elastic.co/downloads/elasticsearch

安装运行

```
$ wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-6.2.2.tar.gz
$ tar xvzf elasticsearch-6.2.2.tar.gz
$ cd elasticsearch-6.2.2
$ ./bin/elasticsearch
```

测试是否安装成功

```
$ curl localhost:9200
{
  "name" : "d0cCcfr",
  "cluster_name" : "elasticsearch",
  "cluster_uuid" : "pDStlLLHQFGaF3_-C0v9Nw",
  "version" : {
    "number" : "6.2.2",
    "build_hash" : "c59ff00",
    "build_date" : "2018-03-13T10:06:29.741383Z",
    "build_snapshot" : false,
    "lucene_version" : "7.2.1",
    "minimum_wire_compatibility_version" : "5.6.0",
    "minimum_index_compatibility_version" : "5.0.0"
  },
  "tagline" : "You Know, for Search"
}
```


## [Mac]安装中文分词插件ik

插件GitHub：https://github.com/medcl/elasticsearch-analysis-ik

安装ik，版本要和elasticsearch的版本完全一致。

```
./bin/elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v6.2.2/elasticsearch-analysis-ik-6.2.2.zip
```



















