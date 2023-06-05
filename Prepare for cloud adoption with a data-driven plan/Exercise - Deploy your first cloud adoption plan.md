
In this exercise, you'll deploy a project plan template to Azure DevOps. That template will give you a sense of the work that needs to be done during this cloud adoption effort. In later exercises, you'll expand that plan to include data gathered from the assessment features of Azure Migrate. This allows you to create a refined plan for both migration and new innovation projects.

## Introduction to the cloud adoption plans

Azure DevOps is the set of cloud-based tools for Azure customers who manage iterative projects. It also includes tools for managing deployment pipelines and other important aspects of DevOps.

In this unit, you'll learn how to quickly deploy a backlog to Azure DevOps by using a template. This template aligns cloud-adoption efforts to a standardized process based on the guidance in the Cloud Adoption Framework for Azure.

## Prerequisites

In Azure DevOps, users have different access levels: basic, stakeholder, or Visual Studio subscriber. Access levels determine what features are available to each user. In order to provision projects by using the demo generator, you need at least a basic access level. For example, you might get an error that indicates the user has a stakeholder license, which doesn't grant permissions to writing shared queries.

### Create an Azure DevOps organization

If you don't have an Azure DevOps organization, you can create one for free.

1. Go to the [Azure DevOps homepage](https://azure.microsoft.com/services/devops/).
    
2. Select **Start Free**.
    
    ![Screenshot of the Azure DevOps home page, with link to Start Free highlighted.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/azure-devops-start-free.png)
    
3. Sign in by using a Microsoft or GitHub account. ![Screenshot of the Azure DevOps sign-in prompt.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/azure-devops-sign-in.png)
    

### Create a new organization in Azure DevOps

If you have an existing Azure DevOps organization but don't have access to create new projects in your organization, you might want to create a new organization to use in this module.

1. [Sign in to the Azure DevOps portal](https://azure.microsoft.com/services/devops/?nav=min), and select **New organization**.
    
    ![Screenshot showing how to create a new organization in Azure DevOps.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/azure-devops-new-org.png)
    
2. Enter a name for the new organization, and select **Continue**. ![Screenshot showing where to enter the name.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/azure-devops-new-org-create.png)
    
3. If the organization has been successfully created, you will see a prompt to **Create a project**.
    
    ![Screenshot that shows the prompt to create a project.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/azure-devops-new-org-project.png)
    

You don't need to create a project at this time. But feel free to do so, if you'd like to get more familiar with Azure DevOps.

## Cloud adoption plan templates

To deploy the cloud adoption plan, open the [Azure DevOps demo generator](https://aka.ms/adopt/plan/generator). As mentioned in the "Prerequisites" section, the demo generator tool requires you to sign in with an account that has proper permissions.

![Screenshot that shows how to sign in to the demo generator.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/demo-generator-sign-in.png)

After you sign in, you can choose a template. There is a growing list of community-led Azure DevOps templates for various purposes, including DevOps labs for demos of features. There are also Microsoft Learn templates, which deploy projects you can use in other Learn modules. You can find the templates containing cloud adoption plans in the **Cloud Adoption Framework** tab.

![Screenshot that shows how to choose a template.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/demo-generator-choose-template.png)

These templates help you plan out work required to implement some of the best practices found in the Cloud Adoption Framework. In this case, choose the **Cloud Adoption Plan** template. This template will load a server migration planning template that you can use throughout this module.

![Screenshot that shows how to select the chosen template.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/demo-generator-select-template.png)

Outside of this module, you can use the cloud adoption plan templates to plan and manage work related to governance, SQL migration, knowledge mining, or other cloud adoption activities.

 Important

The suggested cloud adoption plan template guides activities around migration and closely related upstream or downstream processes. There are a number of other templates that might be more applicable to your cloud adoption efforts. Feel free to use any of those plans during the remainder of this Learn module.

## Deploy your first cloud adoption plan

After you've chosen your template, enter a name for the project (or plan) you want to deploy. We used `DemoForLearnModule` as our project name. You can do the same. Next, choose your DevOps organization. If you don't have one, see the "Prerequisites" section. Then select **Create Project**. ![Screenshot that shows how to create a project from the template.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/demo-generator-create-project.png)

When your project is created, you see a screen like the following. Select **Navigate to project** to open your new project template. ![Screenshot that shows how to open your new project template.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/demo-generator-project-created.png)

## Review your new backlog

When your new project opens, you will have access to a number of different DevOps related features. In this template, you focus specifically on the backlog (or project plans). ![Screenshot that shows where to get familiar with your new project.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/new-project-home.png)

To open the project plan, hover over **Boards** in the left navigation. Then select **Backlogs**. ![Screenshot that shows how to open the backlog.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/new-project-backlogs.png)

The backlog lists all of the different tasks in the project. But there's a better way to look at the project as a whole. In the upper-right corner, select **Stories** > **Epics** to view the full project hierarchy. All of the tasks in this project are now grouped to align to the Cloud Adoption Framework methodologies, or the phases of cloud adoption that you might need throughout your adoption journey.

![Screenshot that shows how to change the view to the Epic hierarchy.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/new-project-epics.png)

This new view is hierarchical. To drill into each phase, select the caret next to any work item. That will expose its child work items.

![Screenshot that shows expanding nodes in the hierarchy.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-plan/media/expanding-nodes.png)

The following list explains Azure DevOps terminology in more traditional project terms:

- **Epic:** In this template, an Epic is a phase of your cloud adoption or digital transformation program.
- **Feature:** In this template, each feature is a project required to complete that phase of adoption.
- **User story:** Each user story is a shared goal or deliverable you will need to be successful when that phase is complete.
- **Task:** Each task is a unit of work that must be done to realize the goal or deliverable.

 Important

Bookmark the address of your new Azure DevOps project in this Epic backlog view. You will need this in the last unit of this Learn module.