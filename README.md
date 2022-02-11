# docker

This repo is an exploratory space for Docker related experiments. 

## CLASSIC COMMANDS - COS WE ALL FORGET SOMETIMES
1. docker ps -all (actively running containers)
2. docker stop {basename}

## Commands 
1. BUILD - `docker build --tag python-docker .`
2. TAGS - `docker tag python-docker:latest python-docker:v1.0.0` 
    - To add version tagging - default = latest
    - NB this does not delete/replace any originally created images. 
    - Remove tagged image - `docker rmi python-docker:v1.0.0`
3. RUN - `docker run --publish 8000:5000 python-docker`
    - [host port]: [container port]
