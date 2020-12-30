[![CircleCI](https://circleci.com/gh/amitdu/udacity-ml.svg?style=svg)](https://app.circleci.com/pipelines/github/amitdu/udacity-ml)

## Project Overview

In this project, I have deployed a Machine Learning Microservice API using Docker and Kubernates. I have also integrate the circleci to lint Dockerfile and API python code via pylint.

## Directory Structure

- `.circleci` : Circleci build configs
- `model_data` : Data used for model training
- `app.py` : Application entrypoint
- `make_prediction.sh` : Shell script for testing prediction API
- `run_docker.sh`: Make docker image build and run locally. 
- `upload_docker.sh`: Tag the image and upload to dockerhub repositry. 
- `run_kubernates.sh`: Run the docker image via K8


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

1. Standalone: `python app.py` : runs onn host at :80 port.
2. Run in Docker: `./run_docker.sh` : It makes docker image and run that docker image and map to 8000 system port.
3. Run in Kubernetes: `./run_kubernetes.sh`: It will run pods at 80 port and map 8000 port to 80.

- The prediction can be tested via `./make_prediction` shell command.
