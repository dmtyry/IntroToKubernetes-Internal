# What The Hack - Intro To Kubernetes
## Introduction
This intro level hack will help you get hands-on experience with Docker, Kubernetes and the Azure Kubernetes Service (AKS) on Microsoft Azure. Kubernetes has quickly gone from being the shiny new kid on the block to the defacto way to deploy and orchestrate containerized applications.

This hack starts off by covering containers, what problems they solve, and why Kubernetes is needed to help orchestrate them.  You will learn all of the Kubernetes jargon (pods, services, and deployments, oh my!).  By the end, you should have a good understanding of what Kubernetes is and be familiar with how to run it on Azure.

## Learning Objectives
In this hack you will solve a common challenge for companies migrating to the cloud. You will take a simple multi-tiered web app, containerize it, and deploy it to an AKS cluster. Once the application is in AKS, you will learn how to tweak all the knobs and levers to scale, manage and monitor it.

1. Containerize an application
1. Deploy a Kubernetes cluster in Azure and deploy applications to it.
1. Understand key Kubernetes management areas: scalability, networking, and monitoring

## Challenges
- Challenge 0: **[Pre-requisites - Ready, Set, GO!](Challenges/00-prereqs.md)**
   - Prepare your workstation to work with Azure, Docker containers, and AKS
- Challenge 1: **[Got Containers?](Challenges/01-containers.md)**
   - Package the app into a Docker container and run it locally.
- Challenge 2: **[The Azure Container Registry](Challenges/02-acr.md)**
   - Deploy an Azure Container Registry and publish your container.
- Challenge 3: **[Introduction To Kubernetes](Challenges/03-k8sintro.md)**
   - Deploy an AKS cluster in Azure and verify it is running.
- Challenge 4: **[Your First Deployment](Challenges/04-k8sdeployment.md)**
   - Pods, Services, Deployments: Getting your YAML on! Deploy the "FabMedical" app to your AKS cluster. 
- Challenge 5: **[Scaling and High Availability](Challenges/05-scaling.md)**
   - Flex Kubernetes' muscles by scaling pods, and then nodes. Observe how Kubernetes responds to resource limits.

## Contributors
- Peter Laudati
- Gino Filicetti
- Israel Ekpo
- Sowmyan Soman Chullikkattil
- Larry Claman
- Dmitrii Tyryshkin
