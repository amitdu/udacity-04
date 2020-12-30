[![CircleCI](https://circleci.com/gh/amitdu/udacity-ml.svg?style=svg)](https://app.circleci.com/pipelines/github/amitdu/udacity-ml)

## Project Overview

In this project, I have deployed a Machine Learning Microservice API using Docker and Kubernates. I have also integrate the circleci to lint Dockerfile and API python code via pylint.

### Project Tasks

I have performed followinng tasks in this project:

- Test your project code using linting
- Complete a Dockerfile to containerize this application
- Deploy your containerized application using Docker and make a prediction
- Improve the log statements in the source code for this application
- Configure Kubernetes and create a Kubernetes cluster
- Deploy a container using Kubernetes and make a prediction
- Upload a complete Github repo with CircleCI to indicate that your code has been tested

---

## Setup the Environment

- Create a virtualenv and activate it
- Run `make install` to install the necessary dependencies

### Running the machine learnning microservice `app.py`

1. Standalone: `python app.py`
2. Run in Docker: `./run_docker.sh`
3. Run in Kubernetes: `./run_kubernetes.sh`

### Kubernetes Steps

- Setup and Configure Docker locally
- Setup and Configure Kubernetes locally
- Create Flask app in Container
- Run via kubectl
