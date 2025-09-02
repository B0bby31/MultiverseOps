
1. Install CRDs for cert-manager:

kubectl apply --server-side --filename https://github.com/prometheus-operator/prometheus-operator/releases/download/v0.84.1/stripped-down-crds.yaml

2. Use the helmfile to sync everything except the flux-instance and flux operator

3. Create external-secrets namespace

4. Create a bitwarden api secret:

  kubectl create secret generic bitwarden-access-token --from-literal=token=<Machine API Token>  -n external-secrets

5. Install the things from external-secrets folder in right order

6. Sync flux-instance and flux-operator

