To deploy to the dev or stage environment, you can use the kustomize command to build the resources with the specific overlays.

Apply to dev environment:
kustomize build ./overlays/dev | kubectl apply -f -


Apply to stage environment:
kustomize build ./overlays/stage | kubectl apply -f -