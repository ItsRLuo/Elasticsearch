# Elasticsearch
Create Elasticsearch instance in minutes

## Setup

1. Run `docker network create elastic`
2. Run `docker run --name es01 --net elastic -p 9200:9200 -v {run_folder_path}/custom_elasticsearch.yml:/usr/share/elasticsearch/config/elasticsearch.yml -it [docker.elastic.co/elasticsearch/elasticsearch:8.6.2](http://docker.elastic.co/elasticsearch/elasticsearch:8.6.2)`
    1. Change `run_folder_path` to your own folder path
3. Open test.html on a browser and you should be able to search
    1. Your index might be empty, you can populate some document using ElasticSearch api or you can use the bulk update api in the insomnia export here
