# terraform-aws-eks

[![Lint Status](https://github.com/terraform-aws-modules/terraform-aws-eks/workflows/Lint/badge.svg)](https://github.com/terraform-aws-modules/terraform-aws-eks/actions)
[![LICENSE](https://img.shields.io/github/license/terraform-aws-modules/terraform-aws-eks)](https://github.com/terraform-aws-modules/terraform-aws-eks/blob/master/LICENSE)

Um módulo terraform para criar um cluster Kubernetes gerenciado no AWS EKS. Inspirado e adaptado de [este documento] (https://www.terraform.io/docs/providers/aws/guides/eks-getting-started.html)
e seu [código-fonte] (https://github.com/terraform-providers/terraform-provider-aws/tree/master/examples/eks-getting-started).
Leia os [documentos da AWS sobre EKS para se conectar ao painel k8s] (https://docs.aws.amazon.com/eks/latest/userguide/dashboard-tutorial.html).

# Premissas

- Você deseja criar um cluster EKS e um grupo de escalonamento automático de trabalhadores para o cluster.
- Você deseja que esses recursos existam em grupos de segurança que permitem a comunicação e a coordenação. Eles podem ser fornecidos pelo usuário ou criados dentro do módulo.
- Você criou uma nuvem privada virtual (VPC) e sub-redes onde pretende colocar os recursos EKS. O VPC atende aos requisitos do EKS.

# Outras documentações

- Autoscaling: How to enable worker node autoscaling.
- Enable Docker Bridge Network: How to enable the docker bridge network when using the EKS-optimized AMI, which disables it by default.
- Spot instances: How to use spot instances with this module.
- IAM Permissions: Minimum IAM permissions needed to setup EKS Cluster.
- FAQ: Frequently Asked Questions

Original code by
Brandon O'Connor. Maintained by Max Williams and Thierno IB. BARRY.
