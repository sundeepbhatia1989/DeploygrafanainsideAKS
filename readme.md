Open Azure CLI and follow these steps. 

mkdir Grafanafolder
 kubectl create namespace grafana-namespace
 cd Grafanafolder/
 nano volume.yaml
 kubectl apply -f volume.yaml
 nano volume.yaml
 kubectl apply -f volume.yaml
 nano volume.yaml
 kubectl apply -f volume.yaml
 nano deployment.yaml
 kubectl apply -f deployment.yaml
 nano service.yaml
 kubectl apply -f service.yaml
 kubectl port-forward --namespace grafana-namespace service/grafana 3000:3000
-------------------
Ref ticket: https://grafana.com/docs/grafana/latest/setup-grafana/installation/kubernetes/#deploy-grafana-enterprise-on-kubernetes
---------------
Run the following command: kubectl apply -f grafana.yaml

Check that it worked by running the following: kubectl port-forward service/grafana 3000:3000

Navigate to localhost:3000 in your browser. You should see a Grafana login page.

Use admin for both the username and password to login.
