# Challenge 4: Your First Deployment

[< Previous Challenge](./03-k8sintro.md) - **[Home](../README.md)** - [Next Challenge >](./05-scaling.md)

## Introduction

Now the rubber meets the road.... we will be deploying the application to our newly minted cluster and making sure it works as intended. You'll learn about pods, deployments and services, oh my!

## Description

In this challenge we need to get our application up and running in Kubernetes. We will learn about Kubernetes configuration YAML files used to create the various Kubernetes resources that will be needed to run our app. 

### Deploy the **API app** using kubectl and YAML files:
- **NOTE:** Sample YAML files to get you started can be found in the Resources folder.
- Deployment details:
  - Number of pods: 2
- Service details:
  - Type: ClusterIP
  - Port and Target Port: 3001
   
### Deploy the Web app using kubectl and YAML files
- **NOTE:** The Web app expects to have an environment variable pointing to the URL of the API app named:
	- **CONTENT_API_URL**
- Create a deployment yaml file for the Web app using the specs from the API app, except for:
	- Port and Target Port: 3000
- Create a service yaml file to go with the deployment
	- **Hint:** Not all "types" of Services are exposed to the outside world
- **NOTE:** Applying your YAML files with kubectl can be done over and over as you update the YAML file. Only the delta will be changed.
- Find out the External IP that was assigned to your service. You can use kubectl for this, or you can look at 'Services' in the Azure portal.
- Test the application by browsing to the Web app's external IP and port and seeing the front page come up.
	- Ensure that you see a list of both speakers and sessions on their respective pages.
	- If you don't see the lists, then the web app is not able to communicate with the API app.

## Success Criteria

1. You have the **content-web** container deployed and can access its page from the open internet.
1. You have the **content-api** container deployed and can get data from the `/speakers` endpoint.
1. The `/speakers` and `/sessions` pages of the content-web display speakers and sessions respectively, not just blank pages.

## Learning Resources
* [Kubernetes Deployment YAMLs explained](https://matthewpalmer.net/kubernetes-app-developer/articles/kubernetes-deployment-tutorial-example-yaml.html)
* [Kubernetes Service Types](https://kubernetes.io/docs/concepts/services-networking/service/#publishing-services-service-types)
* [kubectl cheat sheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)
