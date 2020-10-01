## Example on how to use Prometheus and Grafana to monitor a Flask API application

Example deployment of a Flask API using Prometheus and Grafana for metrics and monitoring. All tied together using docker-compose.


### Set up and run everything using docker-compose

```
docker-compose up
```

### Access

* API: http://<docker-machine-ip>:5000/flask-prometheus-grafana-example/
* Prometheus: http://<docker-machine-ip>:9090/
* Grafana: http://<docker-machine-ip>:3000 `[username: admin, password: pass@123]`
