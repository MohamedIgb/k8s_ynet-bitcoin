# Kubernetes
### The repository includes two apps:
	Ynet app: read the news from http://www.ynet.co.il/Integration/StoryRss2.xml and presents the news into HTML page.
	Bitcoin app: present the current bitcoin price and stores it in redis database, and show the average price for last 10 minutes.

------------

### To run the apps on Minikube:
#### In your terminal
###### clone the repository 
```
git clone https://github.com/MohamedIgb/k8s_ynet-bitcoin.git
```

------------
###### change the directory to the kubernets project
```
cd "path/kubernetes"
```

------------
###### Start Minikube
```
minikube start
```
  

------------

###### Enable ingress addon
```
minikube addons enable ingress
```

------------

###### Apply deployment
```
kubectl apply -f .
```

------------

###### Start minikube tunnel
```
minikube tunnel
```

------------

###### Run from your localhost
	localhost/ynet
  <img width="1440" alt="203833303-aa53d406-4b88-4410-bf51-e6386fcedd21" src="https://user-images.githubusercontent.com/92742400/205567952-9293751e-78ea-43d9-aff4-e24f5276f13c.png">

	localhost/bitcoin
  ![202927832-59960d34-c1db-4a17-b90c-f2a16ea16e3f](https://user-images.githubusercontent.com/92742400/205567991-dd586920-e655-4bcd-9afc-feda06f79a28.jpeg)


