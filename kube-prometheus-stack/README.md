* Creates prometheus, alertmanager and grafana statefulsets.
* Grafana ingress needs to be deployed seperately.
* Change Grafana password.
* Any aditional scrape configs needs to be defined.
* helm install prometheus prometheus-community/kube-prometheus-stack -n monitoring --create-namespace --version 62.3.1
