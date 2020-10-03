## Example on how to use Prometheus and Grafana to monitor a Flask API application and K8S cluster metrics


### Docker compose setup:

```
start docker machine (Quickstart terminal)
docker-compose up
```

### Access

* API: http:// < docker-machine-ip > :5000/flask-prometheus-grafana-example/
* Prometheus: http:// < docker-machine-ip > :9090/
* Grafana: http:// < docker-machine-ip > :3000 `[username: admin, password: pass@123]`

### K8S setup:

```
$ minikube start
$ helm install prom prometheus-community/kube-prometheus-stack
$ kubectl expose deployment prom-grafana --type=LoadBalancer --name mygraph --port=80 --target-port=3000 --protocol=TCP
$ minikube service mygraph --url

Enter your browser at the above URL --> username: admin, password: prom-operator
```
