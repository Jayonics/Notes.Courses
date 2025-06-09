---
title: "LMS | Whizlabs"
source: "https://www.whizlabs.com/learn/course/microsoft-azure-certification-az-400/270/quiz/19448/report/8339063"
author:
published:
created: 2025-06-09
description: "Learning Management System - Whizlabs"
tags:
  - "clippings"
---
![courseimg](https://media.whizlabs.com/website/Microsoft-Azure-DevOps-Solutions-(AZ-400).webp)

Level: Intermediate

Microsoft Azure DevOps Solutions (AZ-400)

[Back to the Course](https://www.whizlabs.com/learn/course/microsoft-azure-certification-az-400/270)

Domain wise Quiz Performance Report

| No. | Domain | Total Question | Correct | Incorrect | Unattempted | Marked for Review |
| --- | --- | --- | --- | --- | --- | --- |
| 1 | Develop a security and compliance plan | 6 | 5 | 1 | 0 | 1 |
| 2 | Design and implement a source control strategy | 6 | 4 | 2 | 0 | 2 |
| 3 | Design and implement build and release pipelines | 28 | 26 | 2 | 0 | 2 |
| 4 | Implement an instrumentation strategy | 8 | 8 | 0 | 0 | 1 |
| 5 | Design and implement processes and communications | 7 | 7 | 0 | 0 | 0 |
| Total | All Domains | 55 | 50 | 5 | 0 | 6 |

Question 1 Marked for review Correct

**Domain:** Design and implement build and release pipelines

Your company has a project in Azure DevOps. The project contains a build pipeline named whizlab-pipeline1 that builds an application named whizlab-app1. You have deployed an agent pool named whizlab-pool that contains a Windows Server 2019 self-hosted agent. The pipeline currently uses whizlab-pool. You have to create another project that would have another build pipeline named whizlab-pipeline2. That pipeline would build another application named whizlab-app2.

Both whizlab-app1 and whizlab-app2 have conflicting dependencies. You have to minimize the possibility of the two build pipelines from conflicting with each other. You also have to minimize infrastructure costs. Which of the following would you implement for this purpose?

- A. Go ahead and create two container jobs.right
- B. Install the self-hosted agent on a Red Hat Enterprise Linux server.
- C. Add another self-hosted agent.
- D. Add a new Docker Compose task to build the pipelines.

###### Explanation:

Answer – A

To save on costs and run applications with conflicting dependencies, you can actually run your applications in containers.

You can run the jobs as containers on the virtual machine. This will ensure that each application can run in isolation and there are no conflicts when it comes to dependencies.

Options B and C are incorrect since these would add to the infrastructure costs.

Option D is incorrect since this is used to build, push or run multi-container Docker applications.

For more information on container jobs, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/process/container-phases?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/container-phases?view=azure-devops)

Question 2 Correct

**Domain:** Design and implement build and release pipelines

You have an Azure DevOps project and an Azure subscription. You have to prevent releases from being deployed unless they comply with the Azure Policies that are assigned to the Azure subscription. Which of the following would you use for this purpose?

- A. A pipeline variable
- B. A deployment gate right
- C. A deployment trigger
- D. A deployment approval

###### Explanation:

Answer – B

In Azure Pipelines, you can define a gate that can ensure the deployment complies with Azure Security policies. When defining a gate in Azure Pipelines, you can actually use the “Security and Compliance assessment task” to check for compliance with Azure Policies.

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on complying with Azure policies for your pipelines, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/policies/azure-policy?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/policies/azure-policy?view=azure-devops)

Question 3 Correct

**Domain:** Design and implement build and release pipelines

You have to use Azure pipelines for building an application. As part of the build process, you have to ensure a group of resources is deployed via an Azure Resource Manager template stored in GitHub. Which of the following would you implement as part of this requirement?

- **Your Answer**
- D. Create a new pipeline
- B. Use the Azure Resource Group deployment task
- E. Define the template parameters
- **Correct Answer**
- B. Use the Azure Resource Group deployment task
- D. Create a new pipeline
- E. Define the template parameters

###### Explanation:

**Correct Answers: B, D and E**

- **Use the Azure Resource Group deployment task**
- **Create a new pipeline**
- **Define the template parameters**
- **Option B is correct:** First, you have to create the release pipeline. Release pipelines can be used to pick ARM templates stored in GitHub.
- **Option D is correct:**Then create the Azure Resource Group deployment task. This will be used for the deployment of the ARM template.
- **Option E is correct:** And then define the template parameters. If the template needs values for parameters in the deployment, then you can specify the template parameters.
- **Option A is incorrect** because the ARM templates can be picked up from GitHub directly, package creation is not required.
- **Option C is incorrect** because the Docker Deploy task is used for deploying Docker applications, it is not used for ARM template deployment.

**Reference:**

- [Use an Azure Resource Manager template to deploy a Linux web app to Azure - Azure Pipelines | Microsoft Docs](https://docs.microsoft.com/en-us/azure/devops/pipelines/apps/cd/azure/deploy-arm-template?view=azure-devops&tabs=json)

Question 4 Correct

**Domain:** Design and implement build and release pipelines

You have a pipeline defined in your Azure DevOps project. You notice that the pipeline fails occasionally. This is because a test measures the response time of an API endpoint that causes the failures. You have to ensure that the build pipeline does not fail because of the test. Which of the following can you carry out to rectify this issue? Choose two answers from the options given below.

- A. Ensure to enable Test impact analysis.
- B. Clear the property of Flaky tests that is included in the test pass percentage.right
- C. Set the Flaky test detection to Off.
- D. Manually go ahead and mark the test as flaky.right

###### Explanation:

Answer – B and D

When you are working with Flaky tests, all of the results are considered in the pipeline. In order to ensure that failures are not included, you have the modify the Project settings in Azure Pipelines. Here you can go ahead and suppress the test failure. You can also manually mark tests as flaky so that they are not considered in the results of the pipeline.

Option A is incorrect because you have to modify the project settings of your Azure DevOps project.

Option C is incorrect because there is no setting to mark the Flaky test detection.

For more information on managing flaky tests, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/test/flaky-test-management?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/test/flaky-test-management?view=azure-devops)

Question 5 Correct

**Domain:** Implement an instrumentation strategy

A company has an Azure subscription that contains several resource groups. The company wants to design a monitoring solution that would provide a consolidated view. The solution needs to adhere to the following requirements.

- Be able to support Role-based access control by using Azure AD identities.
- Be able to includes visuals from Azure Monitor.
- Be able to add documentation that is written in markdown.
- Be able to show the latest data for each visual.

Which of the following would you implement to fulfill these requirements?

- A. Azure Data Explorer
- B. Azure Dashboards right
- C. Azure Monitor
- D. Microsoft Power BI

###### Explanation:

Answer – B

You can organize all of this information within an Azure dashboard. Azure Dashboards provide consolidated views of various aspects such as monitoring your Azure resources or providing an overview of the resources hosted as part of your subscription.

Options A and D are incorrect since these are used for Data Analytics.

Option C is incorrect since this is just the monitoring solution in Azure.

For more information on Azure dashboards, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/azure-portal/azure-portal-dashboards](https://docs.microsoft.com/en-us/azure/azure-portal/azure-portal-dashboards)

Question 6 Correct

**Domain:** Design and implement build and release pipelines

Your company has a set of Azure Pipelines defined. You need to create an integration between Azure Pipelines and Slack. You have to send build notifications to a Slack channel. Which of the following is a step in the implementation plan for achieving this?

- A. Configure a new service connection.
- B. Configure a new service hook subscription.right
- C. Create a new project-level notification.
- D. Create a new organization-level notification.

###### Explanation:

Answer – B

You can achieve this with the help of a service hook subscription. In the service hook, you can subscribe to the Slack channel for a specific event.

Option A is incorrect since you have to create a service hook subscription and not a connection.

Options C and D are incorrect because having notifications will not help. You have to create a service hook subscription to Slack.

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on the integration of Azure DevOps with Slack, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/slack?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/slack?view=azure-devops)

Question 7 Correct

**Domain:** Design and implement processes and communications

Your company has an Azure DevOps project named whizlabs. The project contains pipelines defined in Azure Pipelines that pick up code from GitHub repositories. You have to ensure that developers are able to receive Microsoft Teams notifications when there are failures in the pipeline.

You have to complete the below command for this purpose.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_7-8.png)

Which of the following needs to go into Slot 1?

###### Explanation:

Answer – C

To ensure that you can subscribe to the pipeline, you have to issue the following command @azure pipelines subscribe \[pipeline url\]

Options A, B and D are incorrect because the right way to subscribe is to use the azure pipelines subscribe command.

For more information on the integration of Azure DevOps pipelines with Slack, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/integrations/microsoft-teams?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/integrations/microsoft-teams?view=azure-devops)

Question 8 Correct

**Domain:** Design and implement processes and communications

Your company has an Azure DevOps project named whizlabs. The project contains pipelines defined in Azure Pipelines that pick up code from GitHub repositories. You have to ensure that developers are able to receive Microsoft Teams notifications when there are failures in a build pipeline.

You have to complete the below command for this purpose

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_7-8_13_58.png)

Which of the following needs to go into Slot 2?

- A. https://dev.azure.com/whizlabsorg/whizlabs/
- B. https://dev.azure.com/whizlabsorg/whizlabs/\_build?definitionId=123 right
- C. https://dev.azure.com/whizlabsorg/whizlabs/\_packaging?definitionId=123
- D. https://dev.azure.com/whizlabsorg/whizlabs/\_work\_items?definitionId=123

###### Explanation:

**Answer – B**

As we are targeting a specific pipeline, here you need to give the build URL of that pipeline. The build URL will also have the definition ID for the build to subscribe to.

**Options A is incorrect** because the URL will subscribe to the notifications from all pipelines in the project.

**Option C is incorrect** because they don’t subscribe to the build URL

**Option D is incorrect** because they don’t subscribe to the build URL.

For more information on the integration of Azure DevOps pipelines with Slack, you can refer to the below link

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/integrations/microsoft-teams?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/integrations/microsoft-teams?view=azure-devops)

Question 9 Correct

**Domain:** Design and implement processes and communications

You are a DevOps Engineer for a company using Azure DevOps for project management. The team wants to track the completed story points across sprints to better understand their work capacity and plan future sprints more effectively. You are tasked with determining the average workload a scrum team completes in each sprint.

Which Azure DevOps metric should you use to achieve the goal?

- A. Burndown chart
- B. Cumulative flow diagram
- C. Velocity chart right
- D. Gantt chart

###### Explanation:

**Correct Answer: C**

- **Option C is CORRECT** because a Velocity chart illustrates the work completed by a team in each sprint, typically measured in story points. It indicates the average velocity, representing the average workload a team accomplishes per sprint. This metric is crucial for assessing team capacity and effectively planning future sprints.
- **Option A is INCORRECT** because a Burndown chart tracks the remaining work in a sprint or project over time. It helps teams understand how much work is left and whether they are on track to complete it within the given timeframe. However, it does not provide information on the average amount of work a team completes per sprint.
- **Option B is INCORRECT** because a Cumulative Flow Diagram (CFD) shows the number of work items in each state (e.g., to-do, in-progress, done) over time. It helps identify bottlenecks and understand the workflow but does not directly measure the average amount of work completed per sprint.
- **Option D is INCORRECT** because a Gantt chart is a bar chart that depicts a project schedule, highlighting the start and end dates of tasks and their dependencies. It does not measure the average work completed per sprint. Gantt charts are more commonly used in waterfall project management rather than in agile frameworks like Scrum.

**Reference:**

- [View and configure team velocity - Azure DevOps | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/report/dashboards/team-velocity?view=azure-devops&tabs=in-context)

Question 10 Incorrect

**Domain:** Design and implement build and release pipelines

Your company has an Azure DevOps project and an Azure subscription. Currently, a pipeline is in place that deploys an application to a virtual machine scale set. The scale set sits behind an Azure Standard Load Balancer. The application is accessed via HTTPS only. You need to implement a solution for implementing a health check for the application. This is based on the following requirements.

- Be able to identify whether individual instances in the scale set are eligible for an upgrade operation.
- It should also minimize administrative effort.

Which of the following would you implement for this requirement?

- A. A Custom Script Extension
- B. An Application Health Extension right
- C. Azure Monitor scaling wrong
- D. An Azure Load Balancer health probe

###### Explanation:

Answer – B

This can be achieved by using the Application Health extension. The Health extension can actually view and monitor the health of your underlying instances. And then automatically it also performs the required upgrades on your instances.

Option A is incorrect since this can only install custom scripts on the virtual machine.

Option C is incorrect since this is only a monitoring aspect.

Option D is incorrect since this is only used to monitor the health of the underlying instances sitting behind the load balancer.

For more information on the Application Health extension, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-health-extension](https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-health-extension)

Question 11 Correct

**Domain:** Design and implement build and release pipelines

Your company has the following pipeline definition in Azure DevOps.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_11-12.png)

How many jobs are present in the pipeline?

- A. 0
- B. 1 right
- C. 2
- D. 4

###### Explanation:

Answer – B

There is one job in the pipeline.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_11.png)

Since this is how a job is represented in the pipeline, all other options are incorrect.

For more information on jobs in Azure DevOps, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/process/phases?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/phases?view=azure-devops&tabs=yaml)

Question 12 Correct

**Domain:** Design and implement build and release pipelines

Your company has the following pipeline definition in Azure DevOps.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_11-12_21_15.png)

How many tasks are present in the pipeline?

- A. 0
- B. 1
- C. 2
- D. 4 right

###### Explanation:

Answer – D

There are four tasks in the pipeline.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_12.png)

Since this is how tasks are represented in the pipeline, all other options are incorrect.

For more information on tasks in Azure DevOps, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/process/tasks?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/tasks?view=azure-devops&tabs=yaml)

Question 13 Correct

**Domain:** Develop a security and compliance plan

A company currently has the following resources defined as part of its Azure subscription.

- Windows Server 2019 container images that are stored in Azure Container Registry
- A Log Analytics workspace
- Azure virtual machines that run the latest version of Ubuntu
- An Azure Key vault

For which of the following would you receive security vulnerability assessments? Choose two answers from the options given below.

- A. Windows Server 2019 container images that are stored in Azure Container Registry right
- B. The Log Analytics workspace
- C. Azure virtual machines that run the latest version of Ubuntu
- D. The Azure Key vault right
- E. Microsoft Entra ID

###### Explanation:

**Correct Answers – A & D**

Microsoft Defender for Cloud provides security vulnerability assessments for various resources in your Azure environment.

Microsoft Defender for Cloud supports scanning for Azure container registry images and Azure Key vault, this is also specified in Microsoft documentation:

![](https://s3.amazonaws.com/media.whizlabs.com/learn/MDC.png)

![](https://media.whizlabs.com/website/432900175_1726644098.png)

**Option A is CORRECT** because Microsoft Defender for Cloud supports scanning Azure Container Registry images.

**Option B is incorrect** since there is no support in Microsoft Defender for Cloud for Log Analytics security monitoring.

**Option C is incorrect** because for most of the ubuntu versions, the Microsoft Defender for Cloud service is not available.

**Option D is CORRECT** since "Azure Key vault" has the threat of vulnerability and is supported in Microsoft Defender for Cloud for Entra ID.

**Option E is incorrect** because there is no support from Microsoft Defender for Cloud for Active Directory.

**References:**

[What is Microsoft Defender for Cloud? - Microsoft Defender for Cloud | Microsoft Learn](https://learn.microsoft.com/en-us/azure/defender-for-cloud/defender-for-cloud-introduction#protect-cloud-workloads)

Question 14 Marked for review Correct

**Domain:** Design and implement build and release pipelines

You have an Azure DevOps project that contains a build pipeline. The pipeline builds a container image named whizlabimage and pushes the image to the Azure Container registry. The image uses a base image that is stored in Docker Hub. You have to ensure that whizlabimage is updated automatically whenever the base image is updated. Which of the following can you implement for this requirement?

###### Explanation:

Answer – A

You can use the Azure Container Registry task to check for updates to the base image. The ACR task can be triggered automatically when there is a change to the base image.

Options B and D are incorrect because here we just don’t need a connection or just a hook onto Docker Hub.

Option C is incorrect because Azure Event Hub will look at changes in Azure resources.

For more information on Azure Container Registry tasks, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tasks-overview](https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tasks-overview)

Question 15 Correct

**Domain:** Implement an instrumentation strategy

A company has a set of Azure Virtual Machines that run Windows Server 2019. All of the virtual machines are sending security-related events to a Log Analytics workspace. You have to identify the distinct event ID’s being sent from the different virtual machines.

| **Name** | **Event ID** |
| --- | --- |
| **whizlabvm1** | \[704,701,1501\] |
| **whizlabvm1** | \[326,300,102\] |

You have to design the query for implementing this requirement.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_15-16.png)

Which of the following would go into Slot 1?

- A. count()
- B. project
- C. render
- D. summarize right

###### Explanation:

Answer – D

First, we need to summarize the events. This can be done with the summarize function.

Option A is incorrect because this is used to get the count of records.

Option B is incorrect because this is used to project columns in the results.

Option C is incorrect because this is used to render the results of the query.

For more information on Log Analytics queries, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/azure-monitor/log-query/get-started-queries](https://docs.microsoft.com/en-us/azure/azure-monitor/log-query/get-started-queries)

Question 16 Correct

**Domain:** Implement an instrumentation strategy

A company has a set of Azure Virtual Machines that run Windows Server 2019. All of the virtual machines are sending security-related events to a Log Analytics workspace. You have to identify the distinct event ID’s being sent from the different virtual machines.

| **Name** | **Event ID** |
| --- | --- |
| **whizlabvm1** | \[704,701,1501\] |
| **whizlabvm1** | \[326,300,102\] |

You have to design the query for implementing this requirement.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_15-16_58_10.png)

Which of the following would go into Slot 2?

- A. count() right
- B. project
- C. render
- D. summarize

###### Explanation:

**Answer – A**

Example

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/12/27/ckeditor_111.png)

**Option B is incorrect** because this is used to project columns in the result.

**Option C is incorrect** because this is used to render the results of the query.

**Option D is incorrect** because this is used to summarize the events which come before count().

For more information on Log Analytics queries, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/azure-monitor/log-query/get-started-queries](https://docs.microsoft.com/en-us/azure/azure-monitor/log-query/get-started-queries)

Question 17 Correct

**Domain:** Design and implement build and release pipelines

You have an Azure DevOps project and an Azure subscription. You have a pipeline that is used to build a containerized application. You then deploy that application to a container instance in Azure. You have to ensure to restart the container instance if the application stops working.

You decide to configure a liveness probe to the YAML configuration for the deployment of the application.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

Answer – A

For this requirement, you have the liveness probe that helps to restart broken applications. This probe ensures that the probe only receives traffic when the container is ready to take in requests.

For more information on the liveness probe, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/container-instances/container-instances-liveness-probe](https://docs.microsoft.com/en-us/azure/container-instances/container-instances-liveness-probe)

Question 18 Marked for review Incorrect

**Domain:** Design and implement a source control strategy

You are configuring a branch policy to ensure high-quality code in your Repo by showing requirements for all pull requests.

.

You plan to use Azure Functions to create a custom branch policy for the master branch. You need to ensure that the function inspects the pull request and posts the status to the pull request.

Which of the two settings are required in Azure DevOps? Each correct answer presents a part of the solution.

- A. Add a status policy under branch policies of the master branch.wrong
- B. Configure a service hook for pull request events.right
- C. Add a build policy under branch policies of the master branch.wrong
- D. Create a personal access token with the required scope.right

###### Explanation:

**Answer: B & D**

- **Option A is** **incorrect.** A status policy is used for configuring a branch policy for an external service, so that the service can post the status message to pull requests. In this case, the Azure function code can take care of displaying the message to the pull requests if it is authenticated by DevOps. Communication is set up through a service hook. So, this step is not essential.
- **Option B is** **correct.** To receive an alert when new pull requests are created or to post the status back to the pull request, you need to set up a service hook for pull request events. Service hooks are Azure DevOps Services feature that can alert external services when certain events occur. To receive POST requests when pull requests change, you need to provide the service hook with the Azure function URL.
- **Option C is** **incorrect.** A build policy is required to set up for the code by pre-merging and building pull request changes. Using this, you can mandate an automatic build whenever the source branch is updated. You can also protect the master branch by specifying a policy requirement so that build must succeed to complete pull requests. For setting up a custom branch policy using Azure functions, this is not essential.
- **Option D is** **correct.** To get permission to change pull request status, the azure function must be authenticated with Azure DevOps using a personal access token (PAT). Also, the PAT requires vso.code\_status cope, which you can grant by selecting Code(status) scope on the Create a personal access token page.
- **Reference Link:** For more information on custom branch policies, please refer to the below link- [https://docs.microsoft.com/en-us/azure/devops/repos/git/create-pr-status-server-with-azure-functions?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/create-pr-status-server-with-azure-functions?view=azure-devops)

Question 19 Correct

**Domain:** Design and implement build and release pipelines

You have an Azure DevOps project and an Azure subscription. You have a pipeline used to build a containerized application. You then deploy that application to a container instance in Azure. You have to ensure to restart the container instance if the application stops working.

You decide to configure the IP Flow verify tool in Azure Network Watcher.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

For this requirement, you have the liveness probe that helps to restart broken applications. This probe ensures that traffic is only received by the probe when the container is ready to take in requests.

For more information on the liveness probe, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/container-instances/container-instances-liveness-probe](https://docs.microsoft.com/en-us/azure/container-instances/container-instances-liveness-probe)

Question 20 Correct

**Domain:** Implement an instrumentation strategy

You have an Azure Application Insights availability test configured. You have an Azure Logic App that will be used to send emails. You have to ensure the availability tests invoke the Logic App if there are issues detected via the Availability tests. Which of the following would you setup as the trigger type?

- A. An ApiConnection
- B. A Request trigger
- C. A HTTP Webhook trigger
- D. An HTTP trigger right

###### Explanation:

Answer – D

you can do this by creating a Logic app with an HTTP trigger. You then specify an alert rule in Application Insights and choose 'Run a Logic App from this alert' as the action.  
  
Do you find yourself repeatedly running the same queries on your telemetry data to check whether your service is functioning properly? Are you looking to automate these queries for finding trends and anomalies and then build your own workflows around them? The Azure Application Insights connector for Logic Apps is the right tool for this purpose.

Note

The Azure Application Insights connector has been replaced with the [Azure Monitor connector](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/logicapp-flow-connector) that is integrated with Azure Active Directory instead of requiring an API key and also allows you to retrieve data from a Log Analytics workspace.

With this integration, you can automate numerous processes without writing a single line of code. You can create a logic app with the Application Insights connector to quickly automate any Application Insights process.

You can add additional actions as well. The Logic Apps feature of Azure App Service makes hundreds of actions available. For example, by using a logic app, you can automatically send an email notification or create a bug in Azure DevOps. You can also use one of the many available [templates](https://docs.microsoft.com/en-us/azure/logic-apps/logic-apps-create-logic-apps-from-templates) to help speed up the process of creating your logic app.

Options A, B, and C are incorrect because if you want to use Azure Logic Apps with Azure Monitor, you have to use the An HTTP trigger

For more information on sending alerts in Azure Monitor, you can refer to the below link.  
  
[https://docs.microsoft.com/en-us/azure/azure-monitor/app/automate-with-logic-apps](https://docs.microsoft.com/en-us/azure/azure-monitor/app/automate-with-logic-apps)

Question 21 Correct

**Domain:** Implement an instrumentation strategy

You have a set of Azure Windows Virtual Machines. You have to collect detailed data about the processes running on the guest operating system. Which of the following agents can be used for this requirement? Choose two answers from the options given below.

- A. The Dependency agent right
- B. The Azure Log Analytics agent right
- C. The Azure Network Watcher agent
- D. The Telegraf agent

###### Explanation:

Answer – A and B

You can accomplish this with the help of the Dependency and Azure Log Analytics agent.

The Azure Log Analytics agent can collect information about the virtual machine and then send the data onto a Log Analytics workspace.

The Dependency agent can be used to see the dependency of components hosted on the virtual machines.

Option C is incorrect since this is used for network performance monitoring, diagnostic, and analytics service that allows monitoring of Azure networks.

Option D is incorrect since the Telegraf agent is used to collect performance data from Linux virtual machines.

For more information on the different types of agents, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/azure-monitor/platform/agents-overview](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/agents-overview)

Question 22 Correct

**Domain:** Develop a security and compliance plan View Case Study  

In Contoso Ltd., which access level should be assigned to the CEO (User1) in Azure DevOps to allow viewing of project dashboards and progress without the ability to edit or contribute to the code?

- A. Basic
- B. Stakeholder right
- C. Contributor
- D. Project Administrator

###### Explanation:

**Correct Answer: B**

- **Option B is CORRECT** because the Stakeholder access level is specifically designed for users who need to view and track project progress but do not require permissions to contribute to the code or manage work items. This access level is ideal for executives like the CEO, who need to monitor project statuses, view dashboards, and reports without the risk of altering any project configurations or code. Stakeholders can view boards, backlogs, and dashboards, making it perfect for high-level oversight without involvement in daily operational tasks.
- **Option A is INCORRECT** because the Basic access level provides permissions to contribute to the code and manage work items.
- **Option C is INCORRECT** because the Contributor access level allows for code contributions and work item management, which is beyond what the CEO needs.
- **Option D is INCORRECT** because the Project Administrator access level provides permissions to configure and manage project settings, which is unnecessary for the CEO’s role.

**References:**

- [Stakeholder access quick reference - Azure DevOps | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/organizations/security/stakeholder-access?view=azure-devops)
- [About permissions and security groups - Azure DevOps | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/organizations/security/about-permissions?view=azure-devops&tabs=preview-page)

Question 23 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

Which of the following package feed permissions should be given to the team leads?

- A. Collaborator
- B. Contributor
- C. Owner right
- D. Reader

###### Explanation:

Answer – C

You would need to give Owner privileges so that the team members could edit the feed permissions.

Below is the list of permissions given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_55.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on feed permissions, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/artifacts/feeds/feed-permissions?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/artifacts/feeds/feed-permissions?view=azure-devops)

Question 24 Correct

**Domain:** Design and implement build and release pipelines

A company uses Azure Artifacts for package management. You have to configure an upstream source in Azure Artifacts for Python packages. Which of the following should you use as a repository type as an upstream source?

- A. PyPI right
- B. Npmjs.org
- C. Maven
- D. Third-party trusted Python

###### Explanation:

Answer – A

You can use PyPI, this is used for Python packages.

Option B is incorrect since this is used for Node packages.

Option C is incorrect since this is used for Java packages.

Option D is incorrect since this is not supported in Azure Artifacts.

For more information on getting started with python packages in Azure Artifacts, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/artifacts/quickstarts/python-packages?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/artifacts/quickstarts/python-packages?view=azure-devops)

Question 25 Correct

**Domain:** Design and implement build and release pipelines

You have to deploy Internet Information Services to an Azure virtual machine that runs Windows Server 2019. You have to carry out the deployment using the Desired State Configuration.

You have to complete the below script for this requirement.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_24-25.png)

Which of the following would go into Slot 1?

- A. Configuration right
- B. DependsOn
- C. File
- D. IncludeAllSubFeature
- E. WindowsFeature

###### Explanation:

Answer – A

Here we need to specify the configuration. An example of the IIS configuration is shown below.

```
configuration whizlab
{
    node "localhost"
    {
        WindowsFeature IIS
        {
            Ensure = "Present"
            Name = "Web-Server"
        }
    }
}
```

The other options are incorrect because we have to use the Configuration keyword.

For more information on Desired State Configuration, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/dsc-overview](https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/dsc-overview)

Question 26 Correct

**Domain:** Design and implement build and release pipelines

You have to deploy Internet Information Services to an Azure virtual machine that runs Windows Server 2019. You have to carry out the deployment using the Desired State Configuration.

You have to complete the below script for this requirement.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_24-25_42_20.png)

Which of the following would go into Slot 2?

- A. Configuration
- B. DependsOn
- C. File
- D. IncludeAllSubFeature
- E. WindowsFeature right

###### Explanation:

**Answer – E**

Here we need to specify the WindowsFeature option.

An example of the IIS configuration is shown below.

```
configuration whizlab
{
    node "localhost"
    {
        WindowsFeature IIS
        {
            Ensure = "Present"
            Name = "Web-Server"
        }
    }
}
```

**Option A is incorrect** because the Configuration is applicable in slot 1.

**Option B is incorrect** because DependsOn is used in the YAML pipeline for specifying the dependencies of the stages.

**Option C is incorrect** because it's not used in DSC syntax.

**Option D is incorrect** because this is used for including all required subfeatures within the features you specify with the Name property

For more information on Desired State Configuration, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/dsc-overview](https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/dsc-overview)

Question 27 Correct

**Domain:** Design and implement build and release pipelines

You have to deploy a new application to an Azure Windows virtual machine using the Desired State Configuration extension. Which of the following are steps that need to be followed to implement the Desired State Configuration?

###### Explanation:

Answer – B, D and F

First, you have to create the PowerShell configuration file. The PowerShell configuration needs to be stored in Azure Blob storage.

Then create a DSC Extension on the virtual machine using the PowerShell configuration file.

Option A is incorrect because you have to use Azure Blob storage and not Azure File Storage.

Option C is incorrect because the configuration file needs to be in PowerShell.

Option E is incorrect because we have to use DSC Extension and not the Custom Script Extension.

For more information on Desired State Configuration, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/dsc-overview](https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/dsc-overview)

Question 28 Correct

**Domain:** Develop a security and compliance plan View Case Study  

For the external contractor (User5) contributing to specific repositories in GitHub, which permission level should be assigned to ensure they can contribute code but cannot manage the repository settings?

- A. Read
- B. Write right
- C. Triage
- D. Admin

###### Explanation:

**Correct Answer: B**

- **Option B is CORRECT** because the Write permission level is designed to allow users to actively contribute to a repository. Users with Write permissions can push changes to the repository, create branches, and submit pull requests. This level of access is ideal for an external contractor who needs to contribute code but should not have the authority to alter repository settings or manage other users. This ensures that User5 can fulfill their role effectively by making necessary code contributions while protecting the repository's integrity and administrative settings.
- **Option A is INCORRECT** because the Read permission only allows viewing of the repository and issues but does not allow code contributions.
- **Option C is INCORRECT** because the Triage permission allows users to manage issues and pull requests but does not allow code contributions.
- **Option D is INCORRECT** because the Admin permission provides full control over the repository, including managing settings and permissions, which exceeds what the external contractor needs.

**Reference:**

- [https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization)

Question 29 Correct

**Domain:** Design and implement build and release pipelines

A company is planning to build the following assets-

- Source code being built by multiple development teams
- Production of large and frequently update binary assets
- A common library that can be used by multiple applications
- A place to store logs from automated tests

You have to identify the right store for each type of asset.

Which of the following would you use for the following requirement?

**“Source code being built by multiple development teams”.**

- A. Azure Artifacts
- B. Azure Pipelines
- C. Azure Repos right
- D. Azure Storage
- E. Azure Test Plans

###### Explanation:

Answer – C

For this requirement, we can use Azure Repos. Azure Repos is used for hosting source code in Azure.

Option A is incorrect because this is used for hosting your application packages.

Option B is incorrect because this is used to host your continuous integration and deployment pipelines.

Option D is incorrect because this is used for hosting Blobs in Azure.

Option E is incorrect because this is used for Test Management.

For more information on Azure Repos, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/repos/get-started/what-is-repos?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/get-started/what-is-repos?view=azure-devops)

Question 30 Correct

**Domain:** Design and implement build and release pipelines

A company is planning to build the following assets-

- Source code being built by multiple development teams
- Production of large and frequently update binary assets
- A common library that can be used by multiple applications
- A place to store logs from automated tests

You have to identify the right store for each type of asset.

Which of the following would you use for the following requirement?

**“A common library that can be used by multiple applications”.**

- A. Azure Artifacts right
- B. Azure Pipelines
- C. Azure Repos
- D. Azure Storage
- E. Azure Test Plans

###### Explanation:

Answer – A

For this requirement, we can use Azure Artifacts. This can be used for hosting common application libraries.

Option B is incorrect because this is used to host your continuous integration and deployment pipelines.

Option C is incorrect because this is used for hosting your source code.

Option D is incorrect because this is used for hosting Blobs in Azure.

Option E is incorrect because this is used for Test Management.

For more information on Azure Artifacts, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/artifacts/overview?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/artifacts/overview?view=azure-devops)

Question 31 Correct

**Domain:** Design and implement build and release pipelines

A company is planning to build the following assets-

- Source code being built by multiple development teams
- Production of large and frequently update binary assets
- A common library that can be used by multiple applications
- A place to store logs from automated tests

You have to identify the right store for each type of asset.

Which of the following would you use for the following requirement?

**“A place to store logs from automated tests”**

- A. Azure Artifacts
- B. Azure Pipelines
- C. Azure Repos
- D. Azure Storage
- E. Azure Test Plans right

###### Explanation:

Answer – E

When you run your tests in Azure Test Plans, you can see the logs in the test results.

Option A is incorrect because this is used for hosting your application packages.

Option B is incorrect because this is used to host your continuous integration and deployment pipelines.

Option C is incorrect because this is used for hosting your source code.

Option D is incorrect because this is used for hosting Blobs in Azure.

For more information on Azure Test – automated tests, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/test/run-automated-tests-from-test-hub?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/test/run-automated-tests-from-test-hub?view=azure-devops)

Question 32 Correct

**Domain:** Develop a security and compliance plan View Case Study  

How should Contoso Ltd. configure its Azure DevOps projects to align with its organizational structure, considering they have distinct projects for Marketing and IT?

- A. Create a single project for all teams and manage work using areas and iterations
- B. Create separate projects for Marketing and IT, and configure teams within each project accordingly right
- C. Use a single team for all projects and assign work items based on tags
- D. Create multiple projects based on the geographical distribution of the teams

###### Explanation:

**Correct Answer: B**

- **Option B is CORRECT** because creating separate projects for Marketing and IT aligns with the distinct organizational structure of Contoso Ltd. This approach allows each department to have a dedicated project space, which facilitates focused management and clear oversight of activities, resources, and deliverables specific to each domain. Configuring teams within each project ensures that members have appropriate access to the tools, resources, and work items relevant to their specific functions. This structure supports better organization, tracking, and management of work, and it aligns with best practices for managing multiple, distinct projects within an organization.
- **Option A is INCORRECT** because managing all work in a single project with areas and iterations can complicate management and does not reflect the clear organizational separation.
- **Option C is INCORRECT** because using a single team for all projects and assigning work items based on tags can lead to confusion and inefficiency, especially in large organizations.
- **Option D is INCORRECT** because the separation based on geographical distribution does not align with the logical division of Marketing and IT.

**Reference:**

- [About projects and scaling your organization - Azure DevOps](https://learn.microsoft.com/en-us/azure/devops/organizations/projects/about-projects?view=azure-devops)

Question 33 Correct

**Domain:** Design and implement processes and communications

Your company has a private project in Azure DevOps. You have to ensure that a project manager can create custom work item queries that can be used to report on the project’s progress. The solution must use the principle of least privilege. To which security group must you add the project manager to?

- A. Project Collection Administrators
- B. Readers
- C. Contributors right
- D. Project Administrators

###### Explanation:

**Correct Answer – C**

Considering the principle of least privilege, users with " **Contributors** " permissions can create and save managed My queries, and query charts so the project manager needs to be added to the Readers group.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/Web-capture-10-1-2023-11260-learn.microsoft.com.jpeg)

**Option A is incorrect** because with Project Collection Administrator permission user gets admin-level access which is not required for the current requirement.

**Option B is incorrect** because with "Readers" role does not have the permission to create custom queries.

**Option D is incorrect** because with Project Administrator permission user gets admin access to the project.

**Reference: For more information on query permissions, you can refer to the below link-**

[Set query permissions in Azure Boards and Azure DevOps - Azure Boards | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/boards/queries/set-query-permissions?view=azure-devops#default-query-permissions)

Question 34 Correct

**Domain:** Design and implement build and release pipelines

Your company has an Azure DevOps project that includes package feeds. You have to ensure that a team of developers can unlist and deprecate packages. You have to ensure that the solution used the principle of least privilege. Which of the following would you grant as the access level?

- A. Reader
- B. Collaborator
- C. Contributor right
- D. Owner

###### Explanation:

Answer – C

For this requirement, you can provide the Contributor permission. The Contributor permission permits you to Unlist and deprecate packages.

Options A and B are incorrect since these will not give you the required permissions.

Option D is incorrect since this will not follow the principle of least privilege.

For more information on feed permissions, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/artifacts/feeds/feed-permissions?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/artifacts/feeds/feed-permissions?view=azure-devops)

Question 35 Marked for review Correct

**Domain:** Design and implement a source control strategy

Your company uses Azure DevOps for the management of build and release pipelines for applications. A Git repository is used for application source control. You have to implement a pull request strategy that reduces the history volume in the master branch.

You decide to implement a pull request strategy that uses fast-forward merges.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

No, this can not be used to reduce the history volume.  
Here the new commit will not store the combined history.  
Squash Merge reduces the volume.

For more information on git merge, you can refer to the below link-

- [https://docs.gitlab.com/ee/user/project/merge\_requests/squash\_and\_merge.html](https://docs.gitlab.com/ee/user/project/merge_requests/squash_and_merge.html)

Question 36 Correct

**Domain:** Design and implement a source control strategy

Your company uses Azure DevOps for the management of build and release pipelines for applications. A Git repository is used for application source control. You have to implement a pull request strategy that reduces the history volume in the master branch.

You decide to implement a pull request strategy that uses squash merges.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

Answer – A

Squash merge also helps in reducing the history. The squash merge helps in combining the history of the feature and master branch.

For more information on squash merge, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops)

Question 37 Correct

**Domain:** Design and implement a source control strategy

Your company uses Azure DevOps for the management of build and release pipelines for applications. A Git repository is used for application source control. You have to implement a pull request strategy that reduces the history volume in the master branch.

You decide to implement a pull request strategy that uses an explicit merge.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

For this, you should opt for using squash merges in Git.

For more information on squash merge, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops)

Question 38 Incorrect

**Domain:** Design and implement a source control strategy

Your company uses Azure DevOps for the management of build and release pipelines for applications. A Git repository is used for application source control. You have to implement a pull request strategy that reduces the history volume in the master branch.

You decide to implement a pull request strategy that uses a three-way merge.

Would this fulfill the requirement?

- A. Yes wrong
- B. No right

###### Explanation:

Answer – B

For this, you should opt for using squash merges in Git.

For more information on squash merge, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops)

Question 39 Correct

**Domain:** Design and implement build and release pipelines

Your company has a Git repository in Azure Repos. The developers currently bring the changes directly to the master branch. You have to implement the following requirements.

- Ensure that the master branch is protected. Here you need to ensure that new changes are built in the feature branches first.
- Ensure that changes are reviewed and approved by at least one release manager before each merge
- All changes must be brought into the master branch with the use of pull requests.

Which of the following would you implement for this requirement?

- A. Branch policies right
- B. Project settings
- C. Deployment pools
- D. Branch security

###### Explanation:

Answer – A

To ensure that changes are reviewed and a pull request is in place for merges, you can use Branch policies. The Branch policy can enforce for reviews to be carried out in pull requests.

Option B is incorrect because here you can only work with the settings of the project itself.

Option C is incorrect because this is used to manage the virtual machines which are used for deployment.

Option D is incorrect because this can’t be used to enforce rules on pull requests.

For more information on Branch policies, you can refer to the below link-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/branch-policies-overview?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/branch-policies-overview?view=azure-devops)

Question 40 Incorrect

**Domain:** Design and implement build and release pipelines

The following release pipeline has been defined in Azure DevOps.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_39.41.png)

The Artifacts section has been defined to pick up the artifacts from a build pipeline defined in Azure DevOps.

Would the release pipeline be triggered automatically when the associated build pipeline completes the build process?

- A. Yes wrong
- B. No right

###### Explanation:

Answer – B

If you look closely at the Artifacts section, the lightning symbol indicates that the build would not be triggered automatically. When you actually edit the Artifacts section, you can actually see this setting.

For more information on release pipeline triggers, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/release/triggers?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/triggers?view=azure-devops)

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_39.1.png)

If you enable the “Continuous deployment trigger”, the lightning symbol will change accordingly.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_39.2.png)

Question 41 Marked for review Incorrect

**Domain:** Develop a security and compliance plan View Case Study  

Which of the following steps is necessary to integrate Microsoft Defender for Cloud with Azure DevOps to enhance the security of Contoso Ltd.’s development pipeline?

- A. Install the Azure DevOps Security Scanner extension in Azure DevOps wrong
- B. Enable Azure Policy for GitHub integration
- C. Configure a service connection to allow Microsoft Defender for Cloud access to Azure DevOps right
- D. Add security tasks to the YAML pipelines manually

###### Explanation:

**Correct Answer: C**

- **Option C is CORRECT** because configuring a service connection is a crucial step in integrating Microsoft Defender for Cloud with Azure DevOps. This service connection establishes a secure link between Microsoft Defender for Cloud and the Azure DevOps environment, allowing Defender for Cloud to access, monitor, and secure the DevOps resources and pipelines. By setting up this service connection, Contoso Ltd. can leverage Defender for Cloud's advanced security capabilities to continuously assess and protect their development pipeline against threats and vulnerabilities, thereby enhancing overall pipeline security.
- **Option A is INCORRECT** because there is no specific "Azure DevOps Security Scanner" extension required for this integration.
- **Option B is INCORRECT** because enabling Azure Policy for GitHub integration does not directly relate to integrating Defender for Cloud with Azure DevOps.
- **Option D is INCORRECT** because while adding security tasks to YAML pipelines is useful, it does not constitute the full integration required for Microsoft Defender for Cloud.

**Reference:**

- [https://learn.microsoft.com/en-us/azure/defender-for-cloud/quickstart-onboard-devops](https://learn.microsoft.com/en-us/azure/defender-for-cloud/quickstart-onboard-devops)

Question 42 Correct

**Domain:** Develop a security and compliance plan View Case Study  

To automate the analysis of open-source components for vulnerabilities and licensing issues in GitHub, which action should Contoso Ltd. take with Dependabot?

- A. Enable Dependabot security updates in the repository settings right
- B. Install the Dependabot application from the GitHub Marketplace
- C. Add a Dependabot configuration file to each repository
- D. Configure GitHub Actions to run a daily security scan

###### Explanation:

**Correct Answer: A**

- **Option A is CORRECT** because enabling Dependabot security updates in the repository settings is the most direct and efficient way to automate the monitoring and updating of dependencies for security vulnerabilities. This feature is built into GitHub and can be activated through the repository settings. Once enabled, Dependabot automatically checks for vulnerabilities in the project's dependencies and raises pull requests to update them to secure versions. This automation helps ensure that the codebase remains secure without requiring manual intervention.
- **Option B is INCORRECT** because Dependabot is now a native GitHub feature and does not require separate installation from the GitHub Marketplace.
- **Option C is INCORRECT** because while adding a Dependabot configuration file can provide more customized control, enabling security updates in the settings is the primary step for automation.
- **Option D is INCORRECT** because configuring GitHub Actions for security scans can complement Dependabot but is not the primary method for automating dependency updates and vulnerability checks.

**Reference:**

- [https://learn.microsoft.com/en-us/azure/devops/release-notes/roadmap/2024/ghazdo/dependabot](https://learn.microsoft.com/en-us/azure/devops/release-notes/roadmap/2024/ghazdo/dependabot)

Question 43 Correct

**Domain:** Design and implement build and release pipelines

The following release pipeline has been defined in Azure DevOps.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_39.41_46_08.png)

The Artifacts section has been defined to pick up the artifacts from a build pipeline defined in Azure DevOps.

You have to configure the pipeline to ensure that an approval is required before the build can be released to the “Production” stage. Which of the following would you implement to fulfill this requirement?

- A. Add a gate to the “Staging” stage.
- B. Add a gate to the “Production” stage.
- C. Add an approval to “Production” stage.right
- D. Add a task to the “Production” stage.

###### Explanation:

Answer – C

You can easily perform this requirement by adding an approval to the “Production” stage, as shown below.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_40.png)

1. First modify the pre-stage configuration
2. Enable “Pre-deployment approvals”
3. Enter the approvers for the stage

Since this is clear from the implementation, all other options are incorrect.

For more information on defining an approval, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/approvals?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/approvals?view=azure-devops)

Question 44 Correct

**Domain:** Design and implement processes and communications

A company wants to start using Azure DevOps. Three projects have been created in Azure DevOps for different departments. Each department has different requirements for its project management process.

The department-based requirements are given below.

| **Department** | **Requirement** |
| --- | --- |
| **DepartmentA** | Ability to track product backlogs and bugs on a Kanban board. Should be able to break down the product backlog items into tasks on a task board |
| **DepartmentB** | Should be able to track user stories and bugs on a Kanban board. Should be able to track bugs and tasks on a task board. |
| **DepartmentC** | Need to track requirements, change requests, risks and reviews. |

You have to decide on the right process to adopt Azure Boards for each department.

Which of the following would you adopt for DepartmentA?

- A. Agile
- B. CMMI
- C. Scrum right
- D. XP

###### Explanation:

**Answer – C**

Here you want to track the product backlog items on a Kanban board. You should choose the Scrum process.

The Microsoft documentation mentions the following on the process.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_43.png)

Since this is clear from the documentation, all other options are invalid.

For more information on processes available for Azure Boards, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process](https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process)

Question 45 Correct

**Domain:** Design and implement processes and communications

A company wants to start using Azure DevOps. Three projects have been created in Azure DevOps for different departments. Each department has different requirements for their project management process.

The department-based requirements are given below.

| **Department** | **Requirement** |
| --- | --- |
| **DepartmentA** | Ability to track product backlogs and bugs on a Kanban board. Should be able to break down the product backlog items into tasks on a task board |
| **DepartmentB** | Should be able to track user stories and bugs on a Kanban board. Should be able to track bugs and tasks on a task board. |
| **DepartmentC** | Need to track requirements, change requests m risks and reviews. |

You have to decide on the right process to adopt for Azure Boards for each department.

Which of the following would you adopt for DepartmentB?

- A. Agile right
- B. CMMI
- C. Scrum
- D. XP

###### Explanation:

Answer – A

Here you need to track user stories on a Kanban board. You should opt for the Agile process.

The Microsoft documentation mentions the following on the process.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_44.png)

Since this is clear from the documentation, all other options are invalid.

For more information on processes available for Azure Boards, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process](https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process)

Question 46 Correct

**Domain:** Design and implement processes and communications

A company wants to start using Azure DevOps. Three projects have been created in Azure DevOps for different departments. Each department has different requirements for their project management process.

The department-based requirements are given below.

| **Department** | **Requirement** |
| --- | --- |
| **DepartmentA** | Ability to track product backlogs and bugs on a Kanban board. Should be able to break down the product backlog items into tasks on a task board |
| **DepartmentB** | Should be able to track user stories and bugs on a Kanban board. Should be able to track bugs and tasks on a task board. |
| **DepartmentC** | Need to track requirements, change requests, risks and reviews. |

You have to decide on the right process to adopt Azure Boards for each department.

Which of the following would you adopt for DepartmentC?

- A. Agile
- B. CMMI right
- C. Scrum
- D. XP

###### Explanation:

**Answer – B**

Here the department needs a more agile process to track requirements, reviews and change requests. You should use the CMMI process.

The Microsoft documentation mentions the following on the process.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_x.png)

Since this is clear from the documentation, all other options are invalid.

For more information on processes available for Azure Boards, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process](https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process)

Question 47 Correct

**Domain:** Design and implement a source control strategy

A team is currently using a Git-based repository in Azure repositories. The repository is being used for the source code of a web-based application. The repository has a main master branch and many feature topics branches. There is a large volume of feature requests. It is becoming difficult to follow the history of changes to the master branch. You have to design a pull request merge strategy that would meet the following requirements.

- Allows consolidation of all commit histories
- Merge the changes into a single commit

You need to choose the right branching strategy. Which of the following would you choose?

- A. Git fetch
- B. fast-forward merge
- C. slow-merge
- D. squash merge right

###### Explanation:

Answer – D

You can implement this with the squash merge technique.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_46.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on the squash merge technique, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops)

Question 48 Marked for review Correct

**Domain:** Implement an instrumentation strategy View Case Study  

Which of the following SDK packages related to App Center need to be installed for the mobile-based applications? Choose two answers from the options given below.

- A. Microsoft.AppCenter.Analytics right
- B. Microsoft.AppCenter.System
- C. Microsoft.AppCenter.Crashes right
- D. Microsoft.AppCenter.Mobile

###### Explanation:

Answer – A and C

When setting up an application, you have to install the Microsoft.AppCenter.Analytics and Microsoft.AppCenter.Crashes.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_47.png)

Since this is clear from the implementation, all other options are incorrect.

For more information on getting started with Xamarin, please visit the following URL-

- [https://docs.microsoft.com/en-us/appcenter/sdk/getting-started/xamarin](https://docs.microsoft.com/en-us/appcenter/sdk/getting-started/xamarin)

Question 49 Correct

**Domain:** Implement an instrumentation strategy View Case Study  

You have to add the starting code for the OnCreate() method to integrate the AppCenter SDK with the mobile-based applications.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_48.png)

Which of the following would go into Slot1?

- A. System
- B. Analytics right
- C. Runtime
- D. Mobile

###### Explanation:

Answer – B

Here you need to add the Type of “Analytics”.

This is given as the starting documentation when you set up a project in Visual Studio App Center.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_48.1.png)

Since this is clear from the implementation, all other options are incorrect.

For more information on getting started with Xamarin, please visit the following URL-

- [https://docs.microsoft.com/en-us/appcenter/sdk/getting-started/xamarin](https://docs.microsoft.com/en-us/appcenter/sdk/getting-started/xamarin)

Question 50 Correct

**Domain:** Implement an instrumentation strategy View Case Study  

You have to add the starting code for the OnCreate() method to integrate the AppCenter SDK with the mobile-based applications.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_49.png)

Which of the following would go into Slot2?

- A. System
- B. Crashes right
- C. Runtime
- D. Mobile

###### Explanation:

Answer – B

Here you need to add the Type of “Crashes”.

This is given as the starting documentation when you set up a project in Visual Studio App Center.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_49.1.png)

Since this is clear from the implementation, all other options are incorrect.

For more information on getting started with Xamarin, please visit the following URL-

- [https://docs.microsoft.com/en-us/appcenter/sdk/getting-started/xamarin](https://docs.microsoft.com/en-us/appcenter/sdk/getting-started/xamarin)

Question 51 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

You need to comply with the following requirement.

**“The configuration of the virtual machines must remain consistent during the lifecycle of the application”.**

You decide to implement Custom Script extensions.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

Custom Script Extensions are used to install custom software on the virtual machine. But this is not used to maintain the configuration of the virtual machine.

For more information on Custom Script extensions, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/custom-script-windows](https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/custom-script-windows)

Question 52 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

You need to comply with the following requirement.

**“The configuration of the virtual machines must remain consistent during the lifecycle of the application”.**

You decide to implement Azure Automation.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

Answer – A

Yes, you can use the State configuration of Azure Automation to achieve this.

The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_51.png)

For more information on Azure Automation, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/automation/automation-intro](https://docs.microsoft.com/en-us/azure/automation/automation-intro)

Question 53 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

You need to comply with the following requirement.

**“The configuration of the virtual machines must remain consistent during the lifecycle of the application”.**

You decide to implement an Azure virtual machine with Puppet installed.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

Answer – A

You can also implement configuration management using custom tools such as Chef and Puppet.

A guide is available on the Microsoft site mentioning the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_52.png)

For more information on the guide, please visit the following URL-

- [https://info.microsoft.com/rs/157-GQE-382/images/Infrastructure-as-Code-guide-EN-v6\_299129.pdf](https://info.microsoft.com/rs/157-GQE-382/images/Infrastructure-as-Code-guide-EN-v6_299129.pdf)

Question 54 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

You need to define a secret in the release pipeline. The secret can only be used in the “Release” stage of the pipeline.

Where would you define the secret in the pipeline?

- A. In the variables section right
- B. In the secrets section
- C. In the options section
- D. In the pipeline section

###### Explanation:

Answer A

You would define this in the “Variables section”.

This is given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_53.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on variables in Azure pipelines, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops)

Question 55 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

You need to define a secret in the release pipeline. The secret can only be used in the “Release” stage of the pipeline. How would you ensure that the secret is only defined for the “Release stage”?

- A. Add a trigger for the Release stage only.
- B. Add a scope for the variable.right
- C. Add a tag for the variable.
- D. Add it as an option for the Release stage only.

###### Explanation:

Answer – B

You can define a scope for the variable, as shown below.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_54.png)

Since this is clear from the implementation, all other options are incorrect.

For more information on variables in Azure pipelines, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops)