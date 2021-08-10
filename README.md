# microservices-docker
## docker
```bash
is a platafform of containering. we create images( is an archive that has all config an files to a single program needs to run).
we create container througth an image. container is instance of some image.
```

## Build an image
```bash
docker build -t username_docker_hub/image_name .
```

## List process or containers running on docker
```bash
docker ps -a .
```

## push on dockerhub
```bash
docker push username_docker_hub/image_name 

```
## Kubernetes and basic commands

Kubernetes is an open-source container-orchestration system for automating computer application deployment, scaling, and management. It was originally designed by Google and is now maintained by the Cloud Native Computing Foundation.

## create deployment
```bash
  kubectl apply -f archive.yaml
```
## list of deployments
```bash
  kubectl get deployments
```
## list of pods
```bash
  kubectl get pods
```

## list of services
```bash
  kubectl get services
```

## restart deployments
```bash
  kubectl rollout restart name_of_deployment
```
## kubernetes services - concepts
 when we create a pod is not acessible from outside or inside(througth onther service). we must to define service.
 
 service will  allow that the owe pod can be acessible. there is 4 types of services
 
 ## Load balaced
  allow that pod/container can be acessible from outside(ex: url browser).
  
 ## Node Port
 
 ## Cluster IP
   allow that the pod/container comunicate with others pods/containers.
