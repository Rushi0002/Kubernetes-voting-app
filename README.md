# Start minikube

minikube start

# Create pod

kubectl create -f voting-app-pod.yml

# Create service

kubectl create -f voting-app-service.yml

# Check status of pod

kubectl get pods

# Check status of services

kubectl get services

# Check status of pods, services & deployments at same time

kubectl get pods, svc, deployments

# Check url of service

minikube service voting-service --url

# Delete all pods

kubectl delete pods --all <namespace>

# Delete all services

kubectl delete services --all <namespace>

# Create deployment

**Deployment takes care of replicaset as well as pod creation**

kubectl create -f voting-app-deploy.yml

# Scale up deployments

**It created 3 more pods**

kubectl scale deployment voting-app-deploy --replicas=3
