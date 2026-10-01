# Kubernetes Task 2 - Nginx Deployment on AWS EKS

## Objective
Deploy an Nginx application on an Amazon EKS Kubernetes cluster and expose it using an AWS LoadBalancer.

## Technologies Used
- Amazon EKS
- Kubernetes
- kubectl
- eksctl
- Nginx
- AWS LoadBalancer

## Kubernetes Resources

### Deployment
The `deployment.yaml` file creates an Nginx Deployment with one replica.

### Service
The `service.yaml` file creates a Kubernetes LoadBalancer Service to expose Nginx outside the cluster.

## Files
- `deployment.yaml` - Nginx Deployment configuration
- `service.yaml` - Nginx LoadBalancer Service configuration

## Verification

The following commands will be used to verify the deployment:

    kubectl get nodes
    kubectl get deployments
    kubectl get pods -o wide
    kubectl get svc

External access will be verified after the AWS LoadBalancer is provisioned.

## Status
EKS cluster is active. Worker node provisioning is pending AWS EC2 vCPU quota availability.
