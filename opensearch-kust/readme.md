Deploying with Kustomize
Use kubectl with Kustomize to deploy OpenSearch to your Kubernetes cluster.

a. Deploy to Production

kubectl apply -k opensearch-deployment/overlays/production

b. Deploy to Staging

kubectl apply -k opensearch-deployment/overlays/staging