Deploy Using Kustomize
You can deploy the configuration for each environment using kubectl.

Deploy the dev Environment:
kustomize build --enable-helm overlays/dev |kubectl delete -f -


Deploy the prod Environment:
kustomize build --enable-helm overlays/prod |kubectl delete -f -