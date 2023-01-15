[![CircleCI](https://dl.circleci.com/status-badge/img/gh/aastom/ml-microservice-kubernetes/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/aastom/ml-microservice-kubernetes/tree/main)

## Project Overview

This project creates a Microservice API for a Machine Learning model using a Flask app. The API serves predictions on housing prices through API calls, using a pre-trained sklearn model that predicts housing prices in Boston based on features such as the number of rooms in a house and highway access, teacher-to-pupil ratios, etc.

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
3. Run in Kubernetes:  `./run_kubernetes.sh`