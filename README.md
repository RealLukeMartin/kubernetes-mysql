# kubernetes-mysql

#### Build an instance in GPC with

`gcloud compute disks create --size 200GB mysql-ddisk`

#### Create mysql pod

`kubectl create -f mysql.yaml`

Make sure mysql pod is running

`kubectl get pod mysql`

#### Create mysql service

`kubectl create -f mysql-service.yaml`

Get internal Cluster-IP for the mysql service

`kubectl get service mysql`
