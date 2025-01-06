Applying the Overlays
To deploy the Helm chart with the environment-specific customizations, you can use Kustomize to build and apply the configuration.

For dev environment:

kustomize build ./overlays/dev | kubectl apply -f -
This command will:

Use the Helm chart from the base directory.
Apply the custom values-dev.yaml for the dev environment (setting the Nginx image to nginx:dev and replicas to 1).
For prod environment:

kustomize build ./overlays/prod | kubectl apply -f -