# mesh

## camel-k-operator

This is needed because the helm chart doesn't expose WATCH_NAMESPACE. Instead we use kustomise to pull down the helm chart and patch it.