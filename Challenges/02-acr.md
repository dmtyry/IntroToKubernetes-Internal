# Challenge 2: The Azure Container Registry

[< Previous Challenge](./01-containers.md) - **[Home](../README.md)** - [Next Challenge >](./03-k8sintro.md)

## Introduction

Now that we have our application packaged as container images, where do they go?

## Description

In this challenge we will be creating and setting up a new, private, Azure Container Registry. This will be the new home of the containers we just created. We will see later on how Kubernetes will pull our images from this registry.

## Success Criteria

1. You have provisioned a new Azure Container Registry
1. You have deployed your container images to the registry.
1. You can see images in the registry.

## Learning resources

* [Azure Container Registry docs](https://docs.microsoft.com/en-us/azure/container-registry/)
* [How to tag Docker Images](https://docs.docker.com/engine/reference/commandline/tag/)
* [How to push an image to Azure Container Registry](https://docs.microsoft.com/en-us/azure/container-registry/container-registry-get-started-docker-cli?tabs=azure-cli)
