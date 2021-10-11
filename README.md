Sample Kubernetes commands to run 
-------------------------------------

// this command kickstarts the node port service for VOTING_APP and does a rolling update on this cluster. 
kubectl create -f voting-app-deploy.yaml

kubectl create -f voting-app-service.yaml



# gets the status of the service and deployment running 
kubectl get all 


// this command kickstarts the node port service for REDIS_APP and does a rolling update on this cluster. 
kubectl create -f redis-app-deploy.yaml

kubectl create -f redis-app-service.yaml

# gets the status of the service and deployment running 
kubectl get all 

// this command kickstarts the node port service for WORKER_APP and does a rolling update on this cluster. 
kubectl create -f worker-app-deploy.yaml

kubectl create -f worker-app-service.yaml

# gets the status of the service and deployment running 
kubectl get all 


// gets the status for all the deployments
kubectl get deployment 

// this command kickstarts the node port service for WORKERAPP and does a rolling update on this cluster. 
kubectl create -f result-app-deploy.yaml

kubectl create -f result-app-service.yaml

# gets the status of the service and deployment running 
kubectl get deployments, svc


# get the public URL exposed services
minikiube service voting-service --url

minikube service result-service --url 









