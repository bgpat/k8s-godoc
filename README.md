# k8s-godoc
godoc.org on Kubernetes

## usage

1. Get your access token for Github.com
    https://github.com/settings/tokens/new?description=godoc&scopes=public_repo

2. Deploy to your Kubernetes cluster
    
    ```bash
    kubectl apply -f .
    kubectl -n godoc create secret generic godoc --from-literal=GITHUB_TOKEN=your-token-for-github
    ```
