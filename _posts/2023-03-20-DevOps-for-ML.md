---
title: "DevOps principles for ML"
date: 2023-03-20 +0800
categories: [DevOps, ML]
tags: [DevOps, ML]
---
# What is MLOps
The purpose of MLOps is to make the machine learning lifecycle scalable:

```mermaid
	1. Train model
	2. Package model
	3. Validate model
	4. Deploy model
	5. Monitor model
    6. Retrain model
```

## Machine learning operations (MLOps)
• ML includes all the machine learning workloads for which a data scientist is responsible. A data scientist will do:

```mermaid
	1. Exploratory data analysis (EDA)
	2. Feature engineering
	3. Model training and tuning
```

• DEV refers to the software development, which includes:

```mermaid
	1. Plan: Define the model's requirements and performance metrics.
	2. Create: Create the model training and scoring scripts.
	3. Verify: Check for code and model quality.
	4. Package: Get ready for deployment by staging the solution.
```

• OPS refers to operations and includes:

```mermaid
	1. Release: Deploy the model to production.
	2. Configure: Standardize infrastructure configurations with Infrastructure as Code (IaC).
    3. Monitor: Track metrics and ensure the model and infrastructure are performing as expected.
```

# What is DevOps?

## What is CI/CD?

A key concept to achieve automation is CI/CD, which stands for continuous integration and continuous delivery.

### Continuous integration

```mermaid
• Refactoring exploratory code in Jupyter notebooks into Python or R scripts.

• Linting to check for any programmatic or stylistic errors in the Python or R scripts. For example, check whether a line in your script contains fewer than 80 characters.

• Unit testing to check the performance of the content of the scripts. For example, check whether the model generates accurate predictions on a test dataset.
```

Automation tools:  Azure Pipelines in Azure DevOps, or GitHub Actions.

### Continuous delivery

```mermaid
• involves the steps you need to take to deploy a model to production.

• To deploy a model to production, you'll first want to package it and deploy it to a pre-production environment.

• Once deploying the model to the staging phase is successful and without errors, you can approve for the model to be deployed to the production environment.
```

To collaborate on the Python or R scripts to train the model and any necessary code to deploy the model to each environment, you'll use source control.

## Source control

Source control (or version control) is achieved most commonly by working with a Git-based repository. 

With machine learning projects, you're likely to have a repository for each project you have. The repository will include Jupyter notebooks, training scripts, scoring scripts, and pipeline definitions among other things.

Git-based repositories are available by using Azure Repos in Azure DevOps, or a GitHub repository.

To decide who works on which part of the project, it's recommended to use agile planning.

## Agile planning

Agile planning means you isolate work into sprints. Sprints are short time-periods during which you want to achieve part of the project's goals.

The aim is to plan sprints to quickly improve any of the code.

To avoid spending too much time on model training, agile planning can help to scope the project and help get everyone aligned by agreeing on shorter-term outcomes.

To plan your work, you may use a tool like Azure Boards in Azure DevOps, or GitHub issues.

## Infrastructure as code (IaC)

Using Infrastructure as Code (IaC). When you train and deploy models on Azure, IaC means that you define all Azure resources needed in the process in code and the code is stored in a repository.

# DevOps tools

## cloud-hosted Azure DevOps

```mermaid
	• Azure Boards: organizes agile planning by work item tracking, visualization, and reporting.
	• Azure Repos: stores your code in public and private repositories.
	• Azure Pipelines: combines continuous integration (CI) and continuous delivery (CD) by automatically building and testing your code projects.
```

## What is GitHub?

GitHub is an open-source development platform owned by Microsoft, which includes several DevOps tools like:

```mermaid
	• Issues: tracks your work items, feedback, and bugs.
	• Repos: stores public and private code repositories.
	• Actions: allows for creation of automation workflows.
```

## What is Git?

Git is a distributed source control system. Although there are other source control systems, Git is the most popular system available today and widely used for both open-source frameworks and machine learning projects.


## Reference
https://learn.microsoft.com/en-au/training/modules/introduction-development-operations-principles-for-machine-learn/1-introduction

