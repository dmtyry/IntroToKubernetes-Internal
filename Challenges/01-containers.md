# Challenge 1: Got Containers?

[< Previous Challenge](./00-prereqs.md) - **[Home](../README.md)** - [Next Challenge >](./02-acr.md)

## FabMedical Overview
In this set of challenges, you will be using an application called _FabMedical_, which is a medical conference website application.  The application consists of two components, *web* and *api*, both of which are written using nodejs.  These components currently run natively.  Over the course of this hack, you will containerize these applications and deploy them to Kubernetes.

## Introduction

The first step in our journey will be to take our application and package it as a container image using Docker.

## Description

Your coach will provide you two sample Dockerfiles, which will be used to build the container images for your application.

Steps to complete:
- Download the source code for `content-web` and `content-api` into your local folder (use git clone).  
- Review how the provided Dockerfiles correspond to each of these applications.
- Build Docker images for both content-api and content-web
- Run each of the containers separately to verify if it is working
	- **Hint:** Run the containers in 'detached' mode so that they run in the background.
	- **Hint:** When testing API separately, use its "/sessions" and "/speakers" operations.

## If time permits, bonus task

- Run both containers you just built and check that "sessions" and "speakers" are populated. 
	- **Note:** The containers need to run in the same network to talk to each other. 
		- Create a Docker network named "fabmedical"
		- Run each container using the "fabmedical" network
		- **Hint:** Each container you run needs to have a "name" on a network and this is how you access it from other containers on that network.

## Success Criteria

1. You have mapped Dockerfiles to an appropriate app
2. You have built two images from Dockerfiles
3. Your containers run locally (separately or connected)

## Learning Resources

* [What is Dockerfile syntax](https://www.geeksforgeeks.org/what-is-dockerfile-syntax/)
* [Dockerfile reference](https://docs.docker.com/engine/reference/builder/)
* [How to build an image from a Dockerfile](https://docs.docker.com/engine/reference/commandline/build/)
* [How to run a Dockerfile](https://docs.docker.com/engine/reference/commandline/run/)
* [Containers Networking](https://docs.docker.com/engine/tutorials/networkingcontainers/)

