# Project5
Deploying Flask application in AWS EKS
This Capstone project will utilize CI/CD and cloud services learned during the AWS Cloud DevOps Engineer udacity nanodegree.

Project GitHub Repo:
https://github.com/raju-chekar/caps/

Steps:
Create Dockerfile
Circleci pipeline runs lint tests on Dockerfile to ensure Dockerfile is suited to be uploaded to repository
Dockerfile is built locally and uploaded to Docker repository automatically by CircleCi.
EKS cluster is deployed using Cloudformation script.
Docker application which was uploaded to Docker repository is deployed in EKS cluster by using Kubernetes Cli.

Environment:
Deployment Type - Rolling Deployment
CI tool - Circleci
Files
.circleci/config.yml - circleci config file
testscluster.yml - cloud formation script for eks cluster
requirements.txt - python pip requirements list
flaskapp/app.py - application file
Dockerfile - Docker script to build image
Makefile - Project make file
deployment.yml - deploy script

