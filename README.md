[![CircleCI](https://circleci.com/gh/jafman/udacity-devops-project4.svg?style=svg)](https://circleci.com/gh/jafman/udacity-devops-project4)

## Project Overview

In this project, I applied the skills I have acquired in the course to operationalize a Machine Learning Microservice API. 

I was given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. 

---

## Environment Setup

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

### Files in the Repository
- `app.py` - The flask application code
- `Dockerfile` - The docker definition file
- `Makefile` - Group of commands for installing dependecies, testing & linting
- `requirements.txt` - List of dependencies

