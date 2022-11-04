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


# Architectural Diagram (Shows how key parts of the system work)
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/c113e9e2395bb7aafa16d19a259b5b4f0b07459d/media/cd-diagram.png)

Instructions for running the Python project.  How could a user with no context run this project without asking you for any help.  Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

[Project cloned into Azure Cloud Shell](https://github.com/barmalini18/flask-ml-azure-serverless.git)

1. First, create github repository with scaffolding code (simple code with test, makefile and requirements.txt to install flas, pytest and pylint). Test using github action
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/f5a6c215eec33a4d716fa4d18e889579f5769578/media/01.jpg)

2 Login to azure cloud shell, generate ssh key
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/a8d06b461c26b11a8cb0f5c23560e9fea5ac606e/media/02.jpg)

3. Put the ssh key in github repo
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/4d4a8a5f91c58a399ae18ce69fa251352015ce50/media/03.jpg)

4. Connect to github actions, and generate github actions badge

![example workflow](https://github.com/barmalini18/AzureCI/actions/workflows/pythonapp.yml/badge.svg)

5. Clone the github repo in Azure Cloud Shell
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/36be9a472aad5586cc7500802f6fff4b3073d1ff/media/04.jpg)

# Deploy to Azure Webapp

1. Install Python3.7 (required to run the application) by running the Miniconda script and configuring the PATH variable

![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/75d4e56bd345bab5af88a182a95f433d293b8999/media/05.jpg)

2. Run Makefile to install the requirement, test, lint.
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/776d44f7533ee3b418a8fa490ddcac7af3fdde72/media/06.jpg)

3. Create and deploy Azure webapp
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/776d44f7533ee3b418a8fa490ddcac7af3fdde72/media/07.jpg)


4. Make sure the tests running the `make all` command from the `Makefile`pass
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/2392c034d9ff56628c3ca644f696e5111cde6325/media/08.jpg)

5. Check in browser the webapp is running
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/8a9dfee85e8ffa79b8839ef17893a96e3ceeb74d/media/11.jpg)

6. Call the prediction api by calling the provided scripts:
[Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

```bash
udacity@Azure:~$ ./make_predict_azure_app.sh
Port: 443
{"prediction":[20.35373177134412]}
```
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/8a9dfee85e8ffa79b8839ef17893a96e3ceeb74d/media/09.jpg)


* Successful deploy of the project in Azure Pipelines.

1. Create devops project.
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/509842360898e1874e358789f3fdcfae602e184a/media/12.jpg)

2. Create service connection.
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/509842360898e1874e358789f3fdcfae602e184a/media/13.jpg)

3. Create Pipeline.
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/509842360898e1874e358789f3fdcfae602e184a/media/14.jpg)

* Running Azure App Service from Azure Pipelines automatic deployment
![img](https://github.com/barmalini18/flask-ml-azure-serverless/blob/56da21359bf42c4f6a3758ed10db37035d64deab/media/15.jpg)



## Enhancements

Planning to improve the project:

    In the future, the project can be enhanced with data for another cities worldwide
    Current project limited to python3.7. In the future it can be developed with newer Python version so we can use newer machine learning packages.
    The deployment may use docker.
    Develop web and application to use the current api. Develop Mobile version of the application. 


## Demo 

For Youtube screen-cast follow [this](https://youtu.be/bfPRW3fJefg) link


