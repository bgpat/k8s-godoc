# k8s-godoc
godoc.org on Kubernetes

## usage

1. Deploy to your Kubernetes cluster
    
    ```bash
    kubectl apply -f .
    ```

    If `namespace/godoc` didn't exist, retry to execute `kubectl apply`.

3. Set GITHUB_TOKEN (optional)
    
    [Get your access token for GitHub](https://github.com/settings/tokens/new?description=godoc&scopes=public_repo),
    and create a resource `secret/godoc`.
    
    ```bash
    kubectl -n godoc create secret generic godoc --from-literal=GITHUB_TOKEN=your-token-for-github
    ```
