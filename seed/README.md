# Seed Job

In order to instantiate this in a new argocd cluster...

Install ArgoCD (from https://argo-cd.readthedocs.io/en/latest/getting_started/):

`kubectl create namespace argocd`
`kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml`

Get the admin password via k8s:

`kubectl get secret argocd-initial-admin-secret -n argocd -o json | jq '.data.password' -r | base64 -D`

Or via argocd:

`argocd login --core`

`argocd admin initial-password -n argocd`

Create projects ?

Create repositories ?

Create seed application:

`kubectl apply -f seed/argocd-eda-bootstrap.yaml`