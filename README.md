# cdev-do-k8s

cdev uses [project templates](https://cluster.dev/template-development/) to generate users' projects in a desired cloud. DO-k8s is a cdev template that creates and provisions Kubernetes clusters in the DigitalOcean cloud. 

In this repository you will find all information and samples necessary to start a Kubernetes cluster in DO with cdev. 

The resources to be created:

* *(optional, if vpc_id is not set)* VPC for Kubernetes cluster
* DO Kubernetes cluster with addons:
  * cert-manager
  * argocd

## Prerequisites

1. Terraform version 13+
2. DigitalOcean account.
3. [doctl installed](https://docs.digitalocean.com/reference/doctl/how-to/install/).
4. [cdev installed](https://cluster.dev/installation/).

## Quick Start

1. [Configure access to DO](https://cluster.dev/digital-ocean-cloud-provider/) and export required variables.
2. Clone example project:
    ```
    git clone https://github.com/shalb/cdev-do-k8s.git
    cd examples/
    ```
3. Edit variables in the example's files, if necessary.
4. Run `cdev plan`.
5. Run `cdev apply`
6. You can also use [code generator](https://cluster.dev/quick-start/) to create the same example. 
