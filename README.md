_Task 5 – Kubernetes Cluster with Minikube

This task is part of my DevOps internship. The objective was to build a Kubernetes cluster locally using Minikube and deploy a sample app.

 Tools Used

- Minikube  
- Kubectl  
- Docker  

What I Did

1. Started Minikube  
   - Used `minikube start` to create a local cluster.

2. Created a Deployment  
   - Wrote `deployment.yaml` using the image `kicbase/echo-server:1.0`.
   - Deployed using `kubectl apply -f deployment.yaml`.

3. Exposed the App  
   - Wrote service.yaml with NodePort type.
   - Exposed using kubectl apply -f service.yaml.

4. Verified the Setup  
   - Checked pods and services using kubectl get pods and kubectl get services.

5. Accessed the App
   - Got the service URL using minikube service hello-minikube --url.
   - Opened the app in browser.

6. Scaled the App  
   - Scaled to 3 replicas using kubectl scale deployment hello-minikube --replicas=3.

7. Described the Deployment
   - Used kubectl describe deployment hello-minikube to check details.


 Screenshots

- minikube_start.png  
- nano_deployment_yaml.png  
- deployment_applied.png 
- nano_service_yaml.png  
- service_applied.png 
- get_pods_services.png  
- app_browser_access.png  
- scale_deployment.png  
- describe_deployment.png



All YAML files and screenshots are included in this repo.
