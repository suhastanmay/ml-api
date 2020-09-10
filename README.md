[![CircleCI](https://circleci.com/gh/ClaireLee22/Operationalize-a-Machine-Learning-Microservice-API.svg?style=svg)](https://circleci.com/gh/ClaireLee22/Operationalize-a-Machine-Learning-Microservice-API)

## Project Overview
Deploy a containerized Python flask application to serve out predictions (inference) about housing prices through API calls. It uses a a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features. 

## Project Procedure
* Complete a Dockerfile to containerize this application
* Deploy containerized application using Docker and make a prediction
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Test project code using linting
* Upload a complete Github repo with CircleCI to indicate the code has been tested

## Set up environment and install requirements
  ### Create and Activate Virtual Env for the project
  * python3 -m venv <venv_name>
    source <venv_name>/bin/activate
  * run `make install` to install all the dependencies

## Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

## Files 
1. Dockerfile - contains docker commands to create, run the flask application and to export the application to a required output port.
2. run_docker.sh - Automated script to run docker container of flask app localy.
3. upload_docker.sh - Automated script to upload docker to dockerub.
4. run_kubernetes.sh - Script to run the docker for flask app using kubernetes
5. output_txt_files folder contains the output of docker and kubernetes execution of flask app.
