 Apply the Configurations
Once the overlays are set up, you can apply the configurations for the dev and prod environments:

Apply for dev Environment

kustomize build overlays/dev | kubectl apply -f -


Apply for prod Environment

kustomize build overlays/prod | kubectl apply -f -