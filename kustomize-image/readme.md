Final Output
When you apply the overlay with the command:

kustomize build overlays/production | kubectl apply -f -

Kustomize will generate a complete Kubernetes configuration with the image set to nginx:1.21.0 in the deployment.