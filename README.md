# FastAPI Backends Helm Chart

This is my first Helm chart created as part of my Helm learning journey. The chart consists of three FastAPI backends.

## Installation

To install the chart on your cluster, use the following command:

```sh
helm install fastapi fastapi-backends-0.1.0.tgz -n prod --create-namespace
```

## Port Forwarding

To access the application, you can port forward the service using the following command:

```sh
kubectl port-forward svc/fastapi-backends-resume-upload 8003:8003 -n prod
```

Make sure to adjust the port forwarding command for other services as needed.

## Download the Tarball

You can download the tarball of the Helm chart to install it on your cluster.