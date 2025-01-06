Deploying with Kustomize
Now that you have set up the environments, you can deploy the configurations using Kustomize.

For development:
kustomize build overlays/dev | kubectl apply -f -

For production:
kustomize build overlays/prod | kubectl apply -f -