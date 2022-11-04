# flask-ml-azure
Flask. ML. Azure. DevOps
# AzureCI
CI part of Project6, Scaffolding, lynting, tests etc.
Demonstrates the current status of the code in repository.

![example workflow](https://github.com/barmalini18/AzureCI/actions/workflows/pythonapp.yml/badge.svg)

# Overview

In this project, CI/CD is built for Boston house price predictor. The machine learning model as in this udacity repository. This document describes:

    The project plan in trello and spreadsheet
    Architectural diagram
    Clone the github repository in azure cloud shell
    Create and activate the azure webapp
    Create a CI/CD pipeline in azure


# Project Plan


* A link to a Trello board for the project [here](https://trello.com/b/iHS6JeNO/documentation)
* A link to a spreadsheet that includes the original and final project plan [here](https://docs.google.com/spreadsheets/d/1l1EliuHYJEZpyunagz2PYIUMhirqLyhe/edit?usp=sharing&ouid=110205692645048557882&rtpof=true&sd=true)


* Architectural Diagram (Shows how key parts of the system work)
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/c113e9e2395bb7aafa16d19a259b5b4f0b07459d/media/cd-diagram.png)

<TODO:  Instructions for running the Python project.  How could a user with no context run this project without asking you for any help.  Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

* Project running on Azure App Service

* Project cloned into Azure Cloud Shell

* Passing tests that are displayed after running the `make all` command from the `Makefile`

* Output of a test run

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).

* Running Azure App Service from Azure Pipelines automatic deployment

* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

```bash
udacity@Azure:~$ ./make_predict_azure_app.sh
Port: 443
{"prediction":[20.35373177134412]}
```

* Output of streamed log files from deployed application

> 

## Enhancements

<TODO: A short description of how to improve the project in the future>

## Demo 

<TODO: Add link Screencast on YouTube>


