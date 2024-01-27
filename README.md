## Example on how to use Prometheus and Grafana to monitor a Flask API


### Docker compose setup:

Make sure Docker is started 

``` bash
$ git clone https://github.com/Dgotlieb/Flask-prometheus-grafana.git
$ cd Flask-prometheus-grafana
$ docker-compose up
```

### Access

* API URL1: http://127.0.0.1:5000/
* API URL2: http://127.0.0.1:5000/error
* Prometheus: http://127.0.0.1:9090/
* Grafana: http://127.0.0.1:3000   

`[username: admin, password: pass@123]`
