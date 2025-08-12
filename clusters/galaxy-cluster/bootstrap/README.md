When using this helmfile, you have to first create a secret to authenticate with the Bitwarden Secrets Manager (see https://bitwarden.com/help/secrets-manager-kubernetes-operator/#installation).

Moreover, at the moment, you have to create a dockerconfigjson secret so flux can pull from OCIRegistries (see authentication in https://fluxcd.io/flux/cheatsheets/oci-artifacts/ )