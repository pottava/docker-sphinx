# Dockerized [Sphinx](http://www.sphinx-doc.org/en/master/)

[![pottava/sphinx](http://dockeri.co/image/pottava/sphinx)](https://hub.docker.com/r/pottava/sphinx/)

## Supported tags and respective `Dockerfile` links:

・latest ([versions/2.0/base/Dockerfile](https://github.com/pottava/docker-sphinx/blob/master/versions/2.0/base/Dockerfile))  
・2.0 ([versions/2.0/base/Dockerfile](https://github.com/pottava/docker-sphinx/blob/master/versions/2.0/base/Dockerfile))  
・2.0jp ([versions/2.0/jp/Dockerfile](https://github.com/pottava/docker-sphinx/blob/master/versions/2.0/jp/Dockerfile))  
・1.7 ([versions/1.7/base/Dockerfile](https://github.com/pottava/docker-sphinx/blob/master/versions/1.7/base/Dockerfile))  
・1.7jp ([versions/1.7/jp/Dockerfile](https://github.com/pottava/docker-sphinx/blob/master/versions/1.7/jp/Dockerfile))  

## Usage

```
$ docker run --rm -v `pwd`:/doc -w /doc pottava/sphinx:2.0 make html
```
