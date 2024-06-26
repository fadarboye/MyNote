Note
---

kubectl run redis --image=redis123 --dry-run=client -o yaml > redis-definition.yaml

kubectl create -f redis-definition.yaml

kubectl apply -f redis.yaml

kubectl run redis --image=redis --dry-run=client -o yaml 


-------

https://kubernetes.io/docs/reference/kubectl/conventions/

Create an NGINX Pod


"kubectl run nginx --image=nginx

Generate POD Manifest YAML file (-o yaml). Don't create it(--dry-run)

kubectl run nginx --image=nginx --dry-run=client -o yaml

Create a deployment

kubectl create deployment --image=nginx nginx

Generate Deployment YAML file (-o yaml). Don't create it(--dry-run)

kubectl create deployment --image=nginx nginx --dry-run=client -o yaml

Generate Deployment YAML file (-o yaml). Don’t create it(–dry-run) and save it to a file.

kubectl create deployment --image=nginx nginx --dry-run=client -o yaml > nginx-deployment.yaml

Make necessary changes to the file (for example, adding more replicas) and then create the deployment.

kubectl create -f nginx-deployment.yaml"
