# aws-eks-workshop-blueprints

The objective for this repository is create a knowledge base for this workshop

https://catalog.workshops.aws/eks-blueprints-terraform/en-US/010-introduction/what-is-blueprint/benefits

Before start with this workshop you need to execute the instructions on the file INSTRUCTIONS.md


Currently the lab mentio generate a cloud9 env for execute the lab, but the objetive is not used cloud9 because we will install all tools for this workshop


# reference commands
```bash
export AWS_ACCESS_KEY_ID=AWSACCESSKEYID
export AWS_SECRET_ACCESS_KEY=H2Xk2D6a7Xk+KSECREKEY
export AWS_DEFAULT_REGION=us-east-1
export AWS_REGION=us-east-1
export ACCOUNT_ID=$(aws sts get-caller-identity --output text --query Account)

test -n "$AWS_REGION" && echo AWS_REGION is "$AWS_REGION" || echo AWS_REGION is not set

aws sts get-caller-identity --query Arn | grep eks-blueprints-for-terraform-workshop-admin -q && echo "IAM role valid" || echo "IAM role NOT valid"


 terraform --version 
 asdf install terraform latest 
 asdf local terraform latest 
 terraform --version 
 terraform fmt 
 ls -lrta 
 cd terraform-code/
 terraform fmt 
 terraform fmt 
 terraform init 
 terraform plan 
 terraform fmt 
 terraform plan 
 terraform apply 
 terraform apply 
 terraform fmt 
 terraform validate 
 terraform init 
 terraform validate 
 terraform plan 
 terraform apply -auto-aprove 
 terraform apply -auto-approve 
 aws eks --region us-east-1 update-kubeconfig --name terraform-code
 kubectl get pods 
 k get nodes 
 k get nodes 
 terraform fmt
 terraform fmt
 kubernetes/team-riker
 mkdir kubernetes/team-riker
 mkdir kubernetes/team-riker
 mkdir team-riker
 terraform plan 
 terraform plan 
 terraform apply 
 terraform state list module.eks_blueprints.module.aws_eks_teams
 terraform state show 'module.eks_blueprints.module.aws_eks_teams[0].aws_iam_role.platform_team["admin"]'
 k get pods 
 k get nodes 
 kubectl get configmap -n kube-system aws-auth -o yaml
 terraform plan 
 terraform apply -auto-approve 
 aws eks --region us-east-1 update-kubeconfig --name terraform-code  --role-arn arn:aws:iam::226546938873:role/terraform-code-team-riker-access
 k get pods 
 # list nodes ?
 kubectl get nodes
 # List pods in team-riker namespace ?
 kubectl get pods -n team-riker
 # list all pods in all namespaces ?
 kubectl get pods -A
 # can i create pods in kube-system namespace ?
 kubectl auth can-i create pods --namespace kube-system
 # list service accounts in team-riker namespace ?
 kubectl get sa -n team-riker
 # list service accounts in default namespace ?
 kubectl get sa -n default
 # can i create pods in team-riker namespace ?
 kubectl auth can-i create pods --namespace team-riker
 # can i list pods in team-riker namespace ?
 kubectl auth can-i list pods --namespace team-riker
 kubectl get resourcequotas -n team-riker
 terraform apply 
 aws eks --region us-east-1 update-kubeconfig --name terraform-code  --role-arn arn:aws:iam::226546938873:role/terraform-code-admin-access
 k get pods 
 # list nodes ?
 kubectl get nodes
 # List pods in team-riker namespace ?
 kubectl get pods -n team-riker
 # list all pods in all namespaces ?
 kubectl get pods -A
 # can i create pods in kube-system namespace ?
 kubectl auth can-i create pods --namespace kube-system
 # list service accounts in team-riker namespace ?
 kubectl get sa -n team-riker
 # list service accounts in default namespace ?
 kubectl get sa -n default
 # can i create pods in team-riker namespace ?
 kubectl auth can-i create pods --namespace team-riker
 # can i list pods in team-riker namespace ?
 kubectl auth can-i list pods --namespace team-riker
 aws eks list-clusters 
 aws eks 
 aws eks list-clusters 
 aws eks update-kubeconfig --name terraform-code 
 k get pods 
 # list nodes ?
 kubectl get nodes
 # List pods in team-riker namespace ?
 kubectl get pods -n team-riker
 # list all pods in all namespaces ?
 kubectl get pods -A
 # can i create pods in kube-system namespace ?
 kubectl auth can-i create pods --namespace kube-system
 # list service accounts in team-riker namespace ?
 kubectl get sa -n team-riker
 # list service accounts in default namespace ?
 kubectl get sa -n default
 # can i create pods in team-riker namespace ?
 kubectl auth can-i create pods --namespace team-riker
 # can i list pods in team-riker namespace ?
 kubectl auth can-i list pods --namespace team-riker
 terraform fmt 
 terraform fmt 
 terraform init 
 terraform validate 
 terraform plan
 alias taaa="terraform apply -auto-approve" 
 taaa 
 kubectl get all -n argocd
 k top nodes 
 k get pods 
 k get pods -n argod
 k get pods -n argocd
 kubectl get svc argo-cd-argocd-server -n argocd -o json | jq --raw-output '.status.loadBalancer.ingress[0].hostname'
 ubectl get svc argo-cd-argocd-server -n argocd -o json
 kubectl get svc argo-cd-argocd-server -n argocd -o json
 kubectl get svc argo-cd-argocd-server -n argocd -o json | jq --raw-output '.status.loadBalancer.ingress[0].hostname'
 kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d
 terraform fmt 
 taaa 
 k get ns
 k get pods -n team-riker
 k get all -n team-riker
 taaa 
 taaa 
 terraform destroy -target=module.kubernetes_addons -auto-approve
 terraform destroy -auto-approve

```


### Reference code
https://github.com/aws-ia/terraform-aws-eks-blueprints