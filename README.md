[![CircleCI](https://circleci.com/gh/janssenongaigui/mlproj.svg?style=svg)](https://circleci.com/gh/janssenongaigui/mlproj)

## Project Introduction

* This project is about operationalizing a machine learning model using Docker and Kubernetes.

## Files

* model_data/ contains the model which is used to make predictions
* output_txt_files/ contains outputs when running the app using Docker and Kubernetes
* Dockerfile contains the steps taken to set up the app
* Makefile contains necessary steps for installing, linting, etc.
* app.py contains the code to output predictions using the ML model
* make_prediction.sh contains commands to make predictions against the deployed app
* requirements.txt contains the list of packages required by the app
* run_docker.sh contains steps to deploy using Docker
* run_kubernetes.sh contains steps to deploy using Kubernetes
* upload_docker.sh contains steps to upload to Docker hub

## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py` will run the app locally
2. Run in Docker:  `./run_docker.sh` will run the app using Docker
3. Run in Kubernetes:  `./run_kubernetes.sh` will run the app using Kubernetes

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create the app in Container
* Run via kubectl
