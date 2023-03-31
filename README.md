[![Python application test with Github Actions](https://github.com/SedatF/azure-devops/actions/workflows/main.yml/badge.svg)](https://github.com/SedatF/azure-devops/actions/workflows/main.yml)

# Azure DevOps Project: Building a CI/CD Pipeline

# Overview

This project describe the DevOps CI/CD concepts. using Azure pipeline and Github Actions for automating test, build and deploy web application. 

## Project Plan

* The [Trello board](https://trello.com/) is then used for task planning and tracking.
* The [quarterly project plan](../../raw/main/plan/CI-CD_project_plan.xlsx) the steps for building CI-CD pipeline.

## Instructions
The below diagram shows the project architecture.  

![project architecture](screenshot/CI_CD_Project.svg "project architecture")

The source code are in GitHub repo, actually GitHub Actions perform CI. therefore once any change happend on repo the GitHub Actions can atomatically check the code by build and test.

The code was cloned, build and deployed locally to Azure app serive.

Azure pipline perform CI/CD by pulling the code from GitHub, Build, Test and Deploy it to Azure app service.

### Cloning GitHub Repo and Testing Locally

open the Azure cloud shell by using your credential.

Clone project from GitHub and change to the project directory:
```bash
odl_user [~]$ git clone git@github.com:SedatF/azure-devops.git
odl_user [~]$ cd azure-devops
```

Create python virtual env & source :
```bash
odl_user [~/azure-devops]$ python3 -m venv ~/.azure-devops
odl_user [~/azure-devops]$ source ~/.azure-devops/bin/activate
```
