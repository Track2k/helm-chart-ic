# FastAPI Backends Helm Chart

This is my first Helm chart created as part of my Helm learning journey. The chart consists of three FastAPI backends.

## Clone the Repository

First, clone the repository:

```sh
git clone https://github.com/Track2k/helm-chart-ic.git
cd helm-chart-ic
```

## Installation

To install the chart on your cluster, use the following command:

```sh
helm install fastapi fastapi-backends-0.1.0.tgz -n prod --create-namespace
```

## Port Forwarding

To access the application, you can port forward the service using the following command:

```sh
kubectl port-forward svc/fastapi-resume-upload 8003:8003 -n prod
```

Make sure to adjust the port forwarding command for other services as needed.

## Access fastapi swaggerUI

```sh
https://localhost:8003/docs
```