 990  docker-compose -f docker-compose.yaml run --rm terraform init
  991* git add .
  992* git commit -am "docker compose config"
  993* git push --set-upstream origin 13-EKS-IRSA
➜  01-ekscluster-terraform-manifests git:(13-EKS-IRSA) pwd   
/Users/csuarez/csdemo/13-EKS-IRSA/01-ekscluster-terraform-manifests
➜  01-ekscluster-terraform-manifests git:(13-EKS-IRSA) 


unset AWS_VAULT
ws-vault exec csuarez-aws --duration=12h
pwd
/Users/csuarez/csdemo/13-EKS-IRSA/01-ekscluster-terraform-manifests

docker-compose -f docker-compose.yaml run --rm terraform init

#List workspace
docker-compose -f docker-compose.yaml run --rm terraform workspace list
