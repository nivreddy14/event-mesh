Requires ArgoCD:
https://argo-cd.readthedocs.io/en/stable/getting_started/
And get the password out of the secret.

Install the bootstrap application in argo cd:

Create new app

Application Name : EDA Bootstrap
Repo    : https://github.com/craigedmunds/argocd-eda
Type    : git
Branch  : main
Path    : app-of-apps