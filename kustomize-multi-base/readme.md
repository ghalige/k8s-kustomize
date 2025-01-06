Usage
Generate manifests for development environment (e.g., app1):


kustomize build overlays/dev/app1
Generate manifests for production environment (e.g., app2):


kustomize build overlays/prod/app2
This structure keeps your configurations modular and reusable while allowing environment-specific customizations for each base.