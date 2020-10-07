## Installing Elasticsearch 7 with Kibana using Docker Compose

This repo includes a docker-compose.yml file that can be used for setting up a single node Elasticsearch 7 cluster along with Kibana. This one does not have X-Pack security enabled. If you want to know how to enable x-pack security, I have a blog post explaining the process for Elasticsearch version 6.8 (I haven't tested it with version 7 but you can try it out)

https://codingfundas.com/setting-up-elasticsearch-6-8-with-kibana-and-x-pack-security-enabled/index.html


### Pre-Requisites

- Install Docker engine. I would recommend the official site https://docs.docker.com/engine/install/
- Install Docker compose. For this also, I would recommend official site https://docs.docker.com/compose/install/

Once you have install both Docker and Docker Compose and ensured that Docker engine is running, clone this repo and from the project's root directory, run:


```
docker-compose up -d
```

This should bring up the Elasticsearch and Kibana containers. You can verify by running:


```
docker-compose ps
```

The output should list both the containers and their status should be `Up`.