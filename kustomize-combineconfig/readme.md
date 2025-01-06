How combineConfig Works
In the overlays directory, the kustomization.yaml file is responsible for combining different resources. When you specify multiple resources (like in the dev or prod environment), Kustomize will merge them into a single output.

For example, the overlays/dev/kustomization.yaml file combines the app1 and app2 base resources into one Kustomization configuration. Similarly, in the production environment (overlays/prod/kustomization.yaml), we merge the base configurations and also apply patches.


Using combineConfig to Generate Output
Generate combined output for dev environment:

kustomize build overlays/dev


Generate combined output for prod environment:


kustomize build overlays/prod
This example demonstrates how to use combineConfig by defining multiple base configurations (app1 and app2) and merging them in different environments (such as dev and prod). This approach allows you to maintain modular, reusable configurations while easily combining them into customized manifests for different use cases or environments.