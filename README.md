
[![CircleCI](https://circleci.com/gh/NewthingAde/Machine-Learning-Microservice-Kubernetes/tree/main.svg?style=svg)](https://circleci.com/gh/NewthingAde/Machine-Learning-Microservice-Kubernetes/tree/main)

## Project Overview

This project showcases the skills acquired in the Udacity Cloud DevOps Nanodegree program to operationalize a Machine Learning Microservice API.

This project used a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. Details about the data source is taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project improve my ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

The project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will.

* I tested the project code using linting
* I completed a Dockerfile to containerize this application
* I deployed the containerized application using Docker and make a prediction
* I improved the log statements in the source code for this application
* I configured Kubernetes and create a Kubernetes cluster
* I deployed a container using Kubernetes and make a prediction
* I upload a complete Github repo with CircleCI to indicate that my code has been tested

You can find a detailed [project rubric, here](https://review.udacity.com/#!/rubrics/2576/view).

**The final implementation of the project will showcase your abilities to operationalize production microservices.**

---

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m pip install --user virtualenv
# You should have Python 3.7 available in your host. 
# Check the Python path using `which python3`
# Use a command similar to this one:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
```
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run `minikube start`
4. Run `kubectl config view`
5. Run in Kubernetes:  `./run_kubernetes.sh`


### Kubernetes Steps

* Setup and Configure Docker locally
   
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
