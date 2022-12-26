# Machine Learning Microservice on Kubernetes

This repository contains the code and documentation for a machine learning microservice that is deployed on a Kubernetes cluster. The microservice exposes a simple REST API that allows users to send requests and receive predictions from a machine learning model.

## Requirements

- Docker
- Kubernetes
- Python 3.7 or later

## Setup

1. Clone the repository:

2. Navigate to the project directory:

   cd project-ml-microservice-kubernetes

Run the Docker image:

        ./run_docker.sh


Push the Docker image to Docker Hub:`

```bash
upload_docker.sh

```

Deploy the image to the Kubernetes cluster:

     ./run_kubernetes.sh

## API

The API has the following endpoints:

- `POST /predict`: Accepts a JSON request body with the following format:``

```json
{ "input": <input value> }

```

and returns a JSON response with the following format:`

```json
{ "prediction": <prediction value> }

```
