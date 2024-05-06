https://docs.gitlab.com/ee/user/packages/helm_repository/

###### ###### ###### ######

touch helmfile.yaml

mkdir -p envs/dev/values

touch envs/dev/values/univ.yaml

######  helmfile  ######

helm repo add --username zerodistance --password glpat-dxTFQxAzC1PJV-3Ec62y sputnik https://gitlab.sirius.online/api/v4/projects/176/packages/helm/stable

helm repo update

helm repo list

helmfile template

######  push helm package ######

helm plugin install https://github.com/chartmuseum/helm-push

helm repo add --username zerodistance --password glpat-dxTFQxAzC1PJV-3Ec62y sputnik https://gitlab.sirius.online/api/v4/projects/176/packages/helm/stable

helm repo update

helm repo list

cd NOTES/etc/sputnik/charts/

helm cm-push ory-hydra-0.28.0.tgz sputnik