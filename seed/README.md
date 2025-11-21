# Seed Job

In order to instantiate this in a new argocd cluster...

Install ArgoCD (from https://argo-cd.readthedocs.io/en/latest/getting_started/):

`kubectl create namespace argocd`
`kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml`

Create projects ?

Create repositories ?

Create seed application:

`kubectl apply seed/argocd-eda-bootstrap.yaml`