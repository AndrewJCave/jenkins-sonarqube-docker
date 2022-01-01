# jenkins-sonarqube-docker
Repository for a simple docker project to run Jenkins and SonarQube in a docker container
The docker container will run the current lts version of Jenkins and SonarQube with the Adopt JDK 11 java environment

## Requirements

First off we require docker-compose. Tested with docker-compose version 3.9. 

## Get the repo!
Clone or download the repository into a folder on your local environment using the method of your choice, such as :

Use the 'clone or download' button on this web page
Use your favourite Git client to clone the repo
For you 'command line addicts' use the command line to clone the repo


## First boot 

This is very simple, using docker-compose execute the following command from the root of this repository:

`docker-compose up --build`

## Run the container

### Run with default settings
The dockerfile provides some default settings suitable for most use cases - e.g. exposes web container port - 8080 for Jenkins, 9000 for SonarQube.

To run the container with these defaults, simply use the following command from the root of the local repo folder:

`docker-compose run --rm -
