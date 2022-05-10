# mcr-images-demo

The `kustomization.yaml` file in this directory will take the [upstream ingress-nginx config](https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.2.0/deploy/static/provider/cloud/deploy.yaml) and replace the image references with images from MCR.  

To apply it to your cluster, simply run:

```bash
kustomize build | kubectl apply -f -
```

If you'd like to use a different namespace, change `namespace` in the `kustomization.yaml`.

