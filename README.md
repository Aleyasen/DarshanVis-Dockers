# DarshanVis-Dockers
Repository for Darshan docker files

## Requirements
 - [docker-compose](https://docs.docker.com/compose/)
 

## Get Started
1. Download [docker-compose.yml](https://github.com/Aleyasen/DarshanVis-Dockers/blob/master/docker-compose.yml) or clone the repo.
2. Use docker login to access to the private database docker (aleyasen/darshanvis-mysql). For granting access email [aleyase2@illinois.edu](mailto:aleyase2@illinois.edu).
```bash
docker login
```
3. Run the following command in the directory contains docker-compose.yml.
```bash
docker-compose up -d
```
4. Visit [http://localhost:3000](http://localhost:3000)


## Troubleshooting
- If you get this error message: "In file './common.yml' service 'version' doesn't have any configuration options. All top level keys in your docker-compose.yml must map to a dictionary of configuration options.", then you need to update the version of docker-compose that you are using.  docker-compose 1.7.1 will resolve the issue.
- If you get this error message: "ERROR: Error: image aleyasen/darshanvis-mysql not found", then you need to run "docker login" before docker-compose in order to authenticate with your docker hub credentials in order to access private images.  
