kustomize build overlays/dev

We can deploy the customized manifest using the following command.

kustomize build overlays/dev | kubectl apply -f .
You can also use the following kubectl command.

kubectl apply -k overlays/dev



Run the below command again to review the configuration and patches.

kustomize build overlays/prod
Alternatively, you can use Kustomize with the kubectl command as follows.

kubectl kustomize overlays/prod


Review & Apply Patches
If everything looks good we can deploy it now by running the below command.

kustomize build overlays/prod | kubectl apply -f -
Alternatively, you can use the kubectl command as follows.

kubectl apply -k overlays/prod



