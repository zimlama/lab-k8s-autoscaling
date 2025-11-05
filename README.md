# lab-k8s-autoscaling

# Kubernetes Autoscaling Lab

Laboratorio de Kubernetes con autoescalado horizontal (HPA) y despliegue opcional de ArgoCD.

## Pasos
1. Desplegar métricas:
    kubectl apply -f manifests/metrics-server.yaml


2. Desplegar aplicación:
    kubectl apply -f manifests/nginx-deployment.yaml
    kubectl apply -f manifests/nginx-service.yaml


3. Configurar autoescalado:
    kubectl apply -f manifests/hpa.yaml


4. Verificar estado:
    kubectl get nodes
    kubectl get pods
    kubectl get hpa
    kubectl get svc

