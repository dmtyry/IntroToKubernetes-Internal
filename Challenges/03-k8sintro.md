# Challenge 3: Introduction To Kubernetes

[< Previous Challenge](02-acr.md) - **[Home](../README.md)** - [Next Challenge >](./04-k8sdeployment.md)

## Introduction

Now it is time to introduce the container orchestrator we all came for: Kubernetes!

## Description

In this challenge we will be provisioning our first Kubernetes cluster using the Azure Kubernetes Service (AKS).

- Create a new, multi-node AKS cluster with the following specifications:
	- Use the default Kubernetes version used by AKS.
	- Use 2 nodes of DS2_v2 series VMs
	- Node autoscaling is disabled
	- The cluster should use basic default networking (kubenet)
	- The cluster should be attached to your ACR created in Challenge 2.
      - **NOTE:** Attaching an ACR requires you to have Owner or Azure account administrator role on the Azure subscription. If this is not possible then someone who is an Owner can do the attach for you after you create the cluster (use this [link](https://docs.microsoft.com/en-us/azure/aks/cluster-container-registry-integration?tabs=azure-cli#configure-acr-integration-for-existing-aks-clusters)).

## Success Criteria

1. A new, 2-node AKS kubernetes cluster exists.
1. The AKS cluster is attached to target ACR(s)
2. You are able to connect to the cluster with kubectl and list running nodes (alternatively - just play around "Kubernetes Resources" section in Azure portal, we will be using it in the next challenge)

## Learning Resources:

* [Create AKS using Azure Portal](https://docs.microsoft.com/en-us/azure/aks/learn/quick-kubernetes-deploy-portal)
* [Connect to AKS cluster](https://docs.microsoft.com/en-us/azure/aks/learn/quick-kubernetes-deploy-portal#connect-to-the-cluster)
* [Integrate your Azure Kubernetes Cluster with Azure Container Registry](https://docs.microsoft.com/en-us/azure/aks/cluster-container-registry-integration?tabs=azure-cli)
* [What is kubectl?](https://dockerlabs.collabnix.com/kubernetes/beginners/what-is-kubect.html)
* [kubectl cheat sheet](https://www.containiq.com/post/kubectl-cheat-sheet)
