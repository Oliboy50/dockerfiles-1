# Elasticsearch 1.7/2.4

In a docker-compose.yml for 2.4:
```yml
version: '3'
services:
  elasticsearch:
    image: quay.io/continuouspipe/elasticsearch2.4:stable
```
or 1.7:
```yml
version: '3'
services:
  elasticsearch:
    image: quay.io/continuouspipe/elasticsearch1.7:stable
```

In a Dockerfile for 2.4:
```Dockerfile
FROM quay.io/continuouspipe/elasticsearch2.4:stable
```
or 1.7:
```Dockerfile
FROM quay.io/continuouspipe/elasticsearch1.7:stable
```

## How to build
```bash
docker-compose build --pull elasticsearch24 elasticsearch17
docker-compose push elasticsearch24 elasticsearch17
```

## About

This is a Docker image that provides an Elasticsearch service that tracks the upstream Elasticsearch image.

## How to use

As this is based on the library Elasticsearch image, see their README on [The Docker Hub](https://hub.docker.com/_/elasticsearch/).
