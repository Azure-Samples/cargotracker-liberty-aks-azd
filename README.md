
# Deploy Cargo Tracker to Open Liberty on Azure Kubernetes Service (AKS)

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/Azure-Samples/cargotracker-liberty-aks-azd)
[![Open in Dev Containers](https://img.shields.io/static/v1?style=for-the-badge&label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/azure-samples/cargotracker-liberty-aks-azd)

This sample shows you how to deploy an existing Liberty application to AKS using Liberty on AKS solution templates. When you're finished, you can continue to manage the application via the Azure CLI or Azure Portal.

Cargo Tracker is a Domain-Driven Design Jakarta EE application. The application is built with Maven and deployed to Open Liberty running on Azure Kubernetes Service (AKS). The application is exposed by Azure Application Gateway service.   

For quickstart uses the [official Azure offer for running Liberty on AKS](https://aka.ms/liberty-aks), see [Deploy a Java application with Open Liberty or WebSphere Liberty on an Azure Kubernetes Service (AKS) cluster](https://learn.microsoft.com/azure/aks/howto-deploy-java-liberty-app).

[Features](#features) • [Gettting Started](#getting-started) • [Guidance](#guidance)

(include a screenshot of your template's endpoint here-- so users know what it should look like when they're done)

## Important Security Notice (Template Owners, do not remove!)

This template, the application code and configuration it contains, has been built to showcase Microsoft Azure specific services and tools. We strongly advise our customers not to make this code part of their production environments without implementing or enabling additional security features.


<!-- Documentation page is a WIP, this link does not exist yet -->
For a more comprehensive list of best practices and security recommendations for Intelligent Applications, [visit our official documentation](#link)”

## Features

The following technologies are part of the project:

* Java 17
* Maven
* [Azure CLI](https://learn.microsoft.com/en-us/cli/azure/)
* [Azure Developer CLI (azd)](https://learn.microsoft.com/en-us/azure/developer/azure-developer-cli/)

This project framework provides the following features:

* Feature 1
* Feature 2
* ...

## Getting Started

You have a few options for getting started with this template.

* [GitHub codespace](#github-codespaces)
* [Visual Studio Code with remote containers option](#vs-code-dev-containers)
* [Local Development](#local-environment)

All the steps of this lab have been tested in the GitHub CodeSpace. This is the preferred option for running this lab!

### GitHub Codespaces

You can run this template virtually by using GitHub Codespaces. The button will open a web-based VS Code instance in your browser:

1. Open the template (this may take several minutes)
   [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](placeholder)
2. Open a terminal window
3. Sign into your Azure account:

    ```shell
     azd auth login --use-device-code
    ```

4. [any other steps needed for your template]
5. Provision the Azure resources and deploy your code:

    ```shell
    azd up
    ```

6. (Add steps to start up the sample app)

### VS Code Dev Containers

A related option is VS Code Dev Containers, which will open the project in your local VS Code using the [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers):

1. Start Docker Desktop (install it if not already installed)
2. Open the project:
   [![Open in Dev Containers](https://img.shields.io/static/v1?style=for-the-badge&label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](placeholder)
3. In the VS Code window that opens, once the project files show up (this may take several minutes), open a terminal window.
4. Sign into your Azure account:

    ```shell
     azd auth login
    ```

5. [any other steps needed for your template]
6. Provision the Azure resources and deploy your code:

    ```shell
    azd up
    ```

7. (Add steps to start up the sample app)

8. Configure a CI/CD pipeline:

    ```shell
    azd pipeline config
    ```

### Local Environment

#### Prerequisites

(ideally very short, if any)

* Install [azd](https://aka.ms/install-azd)
    * Windows: `winget install microsoft.azd`
    * Linux: `curl -fsSL https://aka.ms/install-azd.sh | bash`
    * MacOS: `brew tap azure/azd && brew install azd`
* OS
* Library version
* This template uses [MODEL 1] and [MODEL 2] which may not be available in all Azure regions. Check for [up-to-date region availability](https://learn.microsoft.com/azure/ai-services/openai/concepts/models#standard-deployment-model-availability) and select a region during deployment accordingly
    * We recommend using [SUGGESTED REGION]
* ...

#### Installation

(ideally very short)

* list of any prerequisites
* ...

#### Quickstart

(Add steps to get up and running quickly)

1. Bring down the template code:

    ```shell
    azd init --template [name-of-repo]
    ```

   This will perform a git clone

2. Sign into your Azure account:

    ```shell
     azd auth login
    ```

3. [Packages or anything else that needs to be installed]

    ```shell
    npm install ...
    ```

4. ...
5. Provision and deploy the project to Azure:

    ```shell
    azd up
    ```

6. (Add steps to start up the sample app)

7. Configure a CI/CD pipeline:

    ```shell
    azd pipeline config
    ```

#### Local Development

Describe how to run and develop the app locally

## Guidance

### Region Availability

This template uses [MODEL 1] and [MODEL 2] which may not be available in all Azure regions. Check for [up-to-date region availability](https://learn.microsoft.com/azure/ai-services/openai/concepts/models#standard-deployment-model-availability) and select a region during deployment accordingly
* We recommend using [SUGGESTED REGION]

### Costs

You can estimate the cost of this project's architecture with [Azure's pricing calculator](https://azure.microsoft.com/pricing/calculator/)

* [Azure Product] - [plan type] [link to pricing for product](https://azure.microsoft.com/pricing/)

### Security

> [!NOTE]
> When implementing this template please specify whether the template uses Managed Identity or Key Vault

This template has either [Managed Identity](https://learn.microsoft.com/entra/identity/managed-identities-azure-resources/overview) or Key Vault built in to eliminate the need for developers to manage these credentials. Applications can use managed identities to obtain Microsoft Entra tokens without having to manage any credentials. Additionally, we have added a [GitHub Action tool](https://github.com/microsoft/security-devops-action) that scans the infrastructure-as-code files and generates a report containing any detected issues. To ensure best practices in your repo we recommend anyone creating solutions based on our templates ensure that the [Github secret scanning](https://docs.github.com/code-security/secret-scanning/about-secret-scanning) setting is enabled in your repos.

## Resources

(Any additional resources or related projects)

* Link to supporting information
* Link to similar sample
* [Develop Python apps that use Azure AI services](https://learn.microsoft.com/azure/developer/python/azure-ai-for-python-developers)
* ...