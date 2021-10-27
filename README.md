# DO-K8s

Cluster.dev uses [stack templates](https://docs.cluster.dev/stack-templates-overview/) to generate users' projects in a desired cloud. DO-K8s is a stack template that creates and provisions Kubernetes clusters in the DigitalOcean cloud. 

In this repository you will find all information and samples necessary to start a Kubernetes cluster on DO with Cluster.dev. 

The resources to be created:

* *(optional, if vpc_id is not set)* VPC for Kubernetes cluster
* DO Kubernetes cluster with addons:
  * cert-manager
  * argocd

## Prerequisites

1. Terraform version 13+
2. DigitalOcean account.
3. [doctl installed](https://docs.digitalocean.com/reference/doctl/how-to/install/).
4. [Cluster.dev client installed](https://docs.cluster.dev/get-started-install/).

## Quick Start

1. [Configure access to DO](https://docs.cluster.dev/examples-do-k8s/#authentication) and export required variables.
2. Clone example project:
    ```
    git clone https://github.com/shalb/cdev-do-k8s.git
    cd examples/
    ```
3. Edit variables in the example's files, if necessary.
4. Run `cdev plan`
5. Run `cdev apply`

