# Simple kubernetes deployment with mongodb
-----
pre-reqs:
ensure you have minikube, kubectl installed

1) run minikube
2) run the following commands:
    `kubectl apply -f mongo-config.yaml`
    `kubectl apply -f mongo-secret.yaml`
    `kubectl apply -f mongo.yaml`
    `kubectl apply -f webapp.yaml`
3) check status with:`kubectl get all`
4) once confirmed that all the services are up and running, run: ` minikube service webapp-service`
5) you should be able to interact with the basic webapp

we are done?