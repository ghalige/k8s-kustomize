Applying the Overlays
To deploy the dev and prod environments, you can use the following commands:

For dev environment:

kustomize build ./overlays/dev | kubectl apply -f -
This command validates and applies the resources with the settings defined in the dev overlay.

For prod environment:

kustomize build ./overlays/prod | kubectl apply -f -
This command validates and applies the resources with the settings defined in the prod overlay.