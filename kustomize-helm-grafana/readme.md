Deploy Using Kustomize
You can deploy the configuration for each environment using kubectl.

Deploy the dev Environment:
kubectl apply -k overlays/dev


Deploy the prod Environment:
kubectl apply -k overlays/prod