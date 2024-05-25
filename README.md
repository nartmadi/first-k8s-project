# My First Kubernetes Project

This [Kubernetes](https://kubernetes.io/docs/home/) project contains the setup for MongoDB and a Web App.

## Installation

To deploy this project, you need to have [kubectl](https://kubernetes.io/docs/tasks/tools/) and [minikube](https://minikube.sigs.k8s.io/docs/start/) installed.

## Usage

**1. Start Minikube:**
```
minikube start
```
**2. Apply the MongoDB ConfigMap:**
```
kubectl apply -f mongo-config.yaml
```
**3. Apply the MongoDB Secret:**
```
kubectl apply -f mongo-secret.yaml
```
**4. Deploy MongoDB and create the service:**
```
kubectl apply -f mongo-deployment-service.yaml
```
**5. Deploy the Web App and create the service:**
```
kubectl apply -f webapp-deployment-service.yaml
```
**6. Get the URL for accessing the Web App:**
```
minikube service webapp-service --url
```
## Tutorial Video

I used this video to learn and apply the concepts in this project:

[![Kubernetes Tutorial](https://img.youtube.com/vi/s_o8dwzRlu4/maxresdefault.jpg)](https://youtu.be/s_o8dwzRlu4)
