---
title: "LMS | Whizlabs"
source: "https://www.whizlabs.com/learn/course/microsoft-azure-certification-az-400/270/quiz/19449/report/8334818"
author:
published:
created: 2025-06-04
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
| 1 | Develop a security and compliance plan | 8 | 6 | 2 | 0 | 2 |
| 2 | Define and implement continuous integration | 1 | 1 | 0 | 0 | 1 |
| 3 | Design and implement a source control strategy | 9 | 8 | 1 | 0 | 1 |
| 4 | Design and implement build and release pipelines | 24 | 23 | 1 | 0 | 1 |
| 5 | Implement an instrumentation strategy | 5 | 4 | 1 | 0 | 1 |
| 6 | Design and implement processes and communications | 8 | 6 | 2 | 0 | 0 |
| Total | All Domains | 55 | 48 | 7 | 0 | 6 |

Question 1 Correct

**Domain:** Implement an instrumentation strategy

Your company currently has an Azure DevOps project. You have to implement Azure pipelines for the build and deployment of various web-based applications. You have to ensure that monitoring data from Application Insights is incorporated in the release pipeline. Which of the following would you implement for this?

- A. Release annotations
- B. Snapshot Debugger
- C. Funnels
- D. Continuous Monitoring right

###### Explanation:

Answer – D

To enable monitoring data to be available in the DevOps pipeline, you can use Continuous monitoring. Here monitoring can be incorporated into the DevOps Pipeline from Application Insights.

Option A is incorrect because Release Annotations is used to check if the changes you made to your application impact the performance of the application.

Option B is incorrect because this is used to take a debug snapshot of your web application.

Option C is incorrect because this is used to check the user’s usage within your application.

For more information on continuous monitoring, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/azure-monitor/app/continuous-monitoring](https://docs.microsoft.com/en-us/azure/azure-monitor/app/continuous-monitoring)

Question 2 Marked for review Incorrect

**Domain:** Develop a security and compliance plan

Your company currently has an Azure DevOps organization and an Azure subscription. They want to implement various security practices when it comes to managing resources in their Azure subscription. The requirements for security implementation are given below.

- Be able to provide just-in-time access to Azure resources.
- Provide time-bound access to resources.

You decide to implement Conditional Access.

Would this fulfill the requirement?

- A. Yes wrong
- B. No right

###### Explanation:

Answer – B

To meet all of these requirements, you have to use Privileged Identity Management. Conditional Access is used to allow access based on certain conditions.

For more information on Privileged Identity Management, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/active-directory/privileged-identity-management/pim-configure](https://docs.microsoft.com/en-us/azure/active-directory/privileged-identity-management/pim-configure)

Question 3 Incorrect

**Domain:** Design and implement processes and communications

Your team has recently adopted DevOps practices and you need to track the time it takes from code being committed to being deployed in production.

This metric is crucial for assessing your team's efficiency in delivering changes.

Which metric should you use to achieve the goal?

- A. Cycle Time wrong
- B. Lead Time right
- C. Mean Time to Resolution (MTTR)
- D. Frequency of Deployment

###### Explanation:

**Correct Answer: B**

- **Option B is CORRECT** because the lead time for changes tracks the duration from the moment code is committed to its deployment in production. This metric is essential for evaluating the development and deployment processes' efficiency, offering valuable insights into how quickly changes are made available to end-users.
- **Option A is INCORRECT** because cycle time measures the time it takes for a work item to move from the start of the work process to completion. In the context of software development, it typically refers to the duration from when a task is started (e.g., coding begins) to when it is completed (e.g., code is merged or tested). While it is useful for understanding the efficiency of individual stages within the development process, it does not specifically measure the time from code commit to production deployment.
- **Option C is INCORRECT** because the mean time to resolution (MTTR) measures the average time it takes to resolve a problem or incident, from the moment it is detected until it is fixed. While MTTR is important for understanding the efficiency of issue resolution and operational responsiveness, it does not measure the time from code commit to production deployment.
- **Option D is INCORRECT** because frequency of deployment measures how often new changes are deployed to production over a given period. This metric helps understand the regularity and pace of deployments, but it does not provide information on the duration from code commit to production deployment.

**Reference:**

- [Cycle Time and Lead Time control charts - Azure DevOps Services](https://learn.microsoft.com/en-us/azure/devops/report/dashboards/cycle-time-and-lead-time?view=azure-devops)

Question 4 Correct

**Domain:** Design and implement a source control strategy

You are developing a product that has multiple versions. The product must be supported for an extended period. You are using GitHub and have two branches created, ‘feature1’ and ‘feature2’ along with the main branch. A bug was reported and fixed in ‘feature2’ and later merged to the master branch. Later it was discovered that the same bug existed in ‘feature1’ as well, and it needs to be fixed.

You need to ensure that the change is backported from master to ‘feature1’ branch. What should be the best way to fix this?

- A. Merge
- B. Cherry pick right
- C. Rebase
- D. Squash merge

###### Explanation:

**Answer: B**

- **Option A is incorrect.** Merging master down into ‘feature1’ would not be a feasible option since it would contain a significant number of commits. That was not intended to be part of that version.
- **Option B is** **correct.** Using git cherry-pick command enables you to apply specific commits from one branch to another. It merely iterates the selected commits and applies them to the target branch as new commits. If necessary, developers can merge any conflicts before completing the merge down to ‘feature1’.
- **Option C is** **incorrect.** Rebasing master to ‘feature1’ takes all the work done on the master branch, and the feature1 branch will have all the latest changes from master. Feature1 branch may not intend to have master branch changes.
- **Option D is** **incorrect.** Squash merge causes the same issue as merge or rebase. It takes all the file changes from master and adds them to a single new commit on the feature1 branch.
- **Reference Link:** For more information on managing software delivery by using a release based workflow in GitHub, please refer to the below documentation from Microsoft- [https://docs.microsoft.com/en-us/learn/paths/az-400-manage-source-control/](https://docs.microsoft.com/en-us/learn/paths/az-400-manage-source-control/)

Question 5 Correct

**Domain:** Design and implement a source control strategy

Your company is planning to use Git for source control. It would be used for the development of a complex application. You have to decide the right-branching model when it comes to adding new functionality to the application.

Which of the following should be used as the Branch lifetime?

- A. Long-lived
- B. Short-lived right
- C. Master-based
- D. Integration-based

###### Explanation:

**Correct Answer – B**

When adding new features to an application, the best practice is to create short-lived feature branches also known as topic branches. This would reduce the complication when it comes to merging the branch onto the main master branch.

**Options A is incorrect** because a long-lived feature branch (LLFB) can be useful, when working on a feature that shouldn't be present in the master branch until it's ready, it will take a significant amount of time. In case the team is working on a complex system, merging changes will be challenging, and the more time we wait for the merge the more challenging it gets. Hence long-lived branches are not useful in this case.

**Option C is incorrect** because, in the case of a master-based branch, all developers are working on one branch, and the code is directly merged in the master branch. Here the control is in hands of developers, small mistakes will directly go to the master branch if the pull request is not adequately reviewed. In the case of a complex system, there are chances of introducing bugs with new code, and these bugs can directly go to the master branch hence this is not a suitable solution here.

**Option D is incorrect** because the integration branch is used to merge changes coming from multiple feature branches, and then these changes are tested here before merging them to master. This will take time and will be a complex process, as we are merging code from multiple branches there are chances of missing some changes in the merge process hence this is not a good option for a complex system.

For more information on git branching, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/git-branching-guidance?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/git-branching-guidance?view=azure-devops)
- [https://git-scm.com/docs/gitworkflows](https://git-scm.com/docs/gitworkflows)
- [https://git-scm.com/book/en/v2/Git-Branching-Branching-Workflows](https://git-scm.com/book/en/v2/Git-Branching-Branching-Workflows)

Question 6 Correct

**Domain:** Design and implement a source control strategy

Your company is planning to use Git for source control. It would be used for the development of a complex application. You have to decide the right-branching model when it comes to adding new functionality to the application.

Which of the following should be used as the Branch type?

- A. Master
- B. Feature right
- C. Integration
- D. Primary

###### Explanation:

Answer – B

When adding new features to an application, you should consider creating Feature branches.

Options A, C and D are incorrect because the correct adopted design practice is to create feature branches for your features.

For more information on git branching, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/git-branching-guidance?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/git-branching-guidance?view=azure-devops)

Question 7 Correct

**Domain:** Design and implement processes and communications

You need to monitor the progress of work items from development to production to ensure a smooth delivery pipeline devoid of delays. The objective is to visualize the flow of work and identify any bottlenecks. Which Azure DevOps feature is best suited for visualizing the flow of work items through the delivery pipeline?

- A. Azure Boards right
- B. Azure Repos
- C. Release Pipelines
- D. Azure Test Plans

###### Explanation:

**Correct Answer: A**

- **Option A is CORRECT** because Azure Boards provides tools like Kanban boards, task boards, and backlogs which are specifically designed to visualize and track the progress of work items. These tools help in identifying bottlenecks by showing the flow of work items through various stages of the delivery pipeline, making it easier to ensure that there are no delays.
- **Option B is INCORRECT** because Azure Repos is primarily used for version control, enabling teams to manage their code repositories using Git or Team Foundation Version Control (TFVC). While it is essential for managing source code and tracking changes, it does not provide the visualization tools needed to track the progress of work items through the delivery pipeline.
- **Option C is INCORRECT** because Release Pipelines is focused on automating the deployment process, enabling continuous delivery of software. While it is crucial for managing and automating releases, it does not provide a comprehensive view of work item progress from development to production, nor does it visualize the flow of work items across different stages.
- **Option D is INCORRECT** because Azure Test Plans is designed for managing and executing test cases, capturing test results, and providing insights into the quality of the product through testing. It is not intended for tracking the overall progress of work items through the delivery pipeline or visualizing the flow of work items.

**References:**

- [https://learn.microsoft.com/en-us/azure/devops/boards/get-started/what-is-azure-boards?view=azure-devops](https://learn.microsoft.com/en-us/azure/devops/boards/get-started/what-is-azure-boards?view=azure-devops)

Question 8 Correct

**Domain:** Design and implement processes and communications

Your company is planning to use Azure DevOps. They want to use Azure DevOps for sprint planning. Here they also want to visualize the flow of work by using agile methodology. Which of the following should they use in Azure DevOps?

- A. Kanban boards right
- B. Sprint planning
- C. Delivery plans
- D. Portfolio backlogs

###### Explanation:

Answer – A

This can be achieved with the use of Kanban boards. With Kanban boards, you can get a visualization of the different work items in your project.

Option B is incorrect since this is only used for planning your sprints.

Option C is incorrect since Delivery plans cannot be used for visualization.

Option D is incorrect since this is used to host your work items.

For more information on Kanban boards, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/boards/boards/kanban-quickstart?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/boards/boards/kanban-quickstart?view=azure-devops)

Question 9 Marked for review Incorrect

**Domain:** Design and implement build and release pipelines

Your company currently uses Azure DevOps to deploy an application to Azure.

The project team has created a pipeline for building and deploying the changes. Below is the execution result of the pipeline.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_9-10.png)

How many stages the team has added to the pipeline?

- A. 1
- B. 2 right
- C. 3 wrong
- D. 4

###### Explanation:

**Answer – B**

The pipeline has two stages. One is the Build and the other is the Deploy phase.

The Finalize build job is the default task performed at the end of the build to update the status, the team did not add it so it can not be considered.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_9.png)

Since this is clear from the implementation, all other options are incorrect.

For more information on stages in Azure Pipelines, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/process/stages?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/stages?view=azure-devops&tabs=yaml)

Question 10 Correct

**Domain:** Design and implement a source control strategy

A company is planning to use Azure DevOps. They need to implement a method that would ensure that the code meets the defined quality and code review standards of the company. Which of the following would you implement for this requirement?

- A. branch locking
- B. branch permissions
- C. branch policies right
- D. branch tagging

###### Explanation:

Answer – C

Branch policies help ensure best practices can be followed when code is checked into a branch. The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2019/09/17/ckeditor_38.png)

Since this is clearly mentioned in the documentation, all other options are incorrect.

For more information on branch policies, one can visit the below URL-

[https://docs.microsoft.com/en-us/azure/devops/repos/git/branch-policies-overview?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/branch-policies-overview?view=azure-devops)

Question 11 Correct

**Domain:** Design and implement build and release pipelines

You have to deploy a Terraform script to Azure for the creation of resources. You have to authenticate Azure with the use of a service principal.

You have to execute the following command for creation of the service principal.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_11-12_17_07.png)

Which of the following would go into Slot 1?

- A. deploy
- B. create
- C. create-for-rbac right
- D. service

###### Explanation:

Answer – C

Here you need to create the service principal with RBAC capabilities.

Options A and D are incorrect since these are not the correct parameters to specify in the command.

Option B is incorrect because we need to ensure that the service principal has RBAC capabilities.

For more information on getting started with Azure Cloud Shell and Terraform, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/developer/terraform/get-started-cloud-shell](https://docs.microsoft.com/en-us/azure/developer/terraform/get-started-cloud-shell)

Question 12 Correct

**Domain:** Design and implement build and release pipelines

You have to deploy a Terraform script to Azure for the creation of resources. For executing terraform and creating the resources on Azure you will first need to authenticate to Azure Portal and for authentication, you will be using service principal.  
You have to execute the following command for the creation of the service principal.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_11-12_21_30.png)

Which of the following values needs to be used in the az login command when using service principal for authentication? (Select THREE)

- A. service principal name right
- B. subscription name
- C. subscription Id
- D. password right
- E. tenant id right

###### Explanation:

**Answer – A, D, and E**

You need to use the service principal name, password, and tenant ID. These are required when you log in with the service principal.

**Options B and C are incorrect** since you don’t have to mention these parameters when you log in with the service principal.

For more information on getting started with Azure Cloud Shell and Terraform, one can browse the following URL-

- [https://docs.microsoft.com/en-us/azure/developer/terraform/get-started-cloud-shell](https://docs.microsoft.com/en-us/azure/developer/terraform/get-started-cloud-shell)
- [https://docs.microsoft.com/en-us/cli/azure/authenticate-azure-cli](https://docs.microsoft.com/en-us/cli/azure/authenticate-azure-cli)

Question 13 Correct

**Domain:** Design and implement a source control strategy

Your company has a Git repository hosted in Azure DevOps.

You have to configure the pull requests in a branch to meet the following requirements before they are merged.

- Ensure that the committed code is compiled successfully.
- Ensure that pull requests have a Quality gate status of passed in SonarCloud.

Which of the following can be used for the requirement?

**“Ensure that committed code is compiled successfully.”**

- A. A build policy right
- B. A check-in policy
- C. A status policy
- D. A deployment policy

###### Explanation:

Answer – A

With Git repositories, you can ensure that a build passes before the code is committed using a build policy.

Option B is incorrect since this is used for Team Foundation Version Control.

Option C is incorrect since this is used for checking for the status of external services.

Option D is incorrect since this is not an option for working with Azure Repos.

For more information on build validation, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/branch-policies?view=azure-devops#build-validation](https://docs.microsoft.com/en-us/azure/devops/repos/git/branch-policies?view=azure-devops#build-validation)

Question 14 Correct

**Domain:** Implement an instrumentation strategy

You query a log table using KQL. You need to filter the input table on condition and select columns for your result table.

What two operators will you use in your query?

- A. render
- B. summarize
- C. project right
- D. let
- E. find
- F. extend
- G. where right
- H. set

###### Explanation:

**Correct Answers: C and G**

Microsoft Azure Monitor stores two types of data: logs and metrics. This data helps users monitor, tune, and troubleshoot their applications and services. Azure Monitor collects data from applications, operating systems, Azure resources, subscriptions, tenants, and custom sources.

Logs data are the records that contain predominantly text information but can include numeric data as well. Typically, logs store event information from a variety of sources. Azure Monitor creates a table for each log source to store its data and uses Log Analytics workspace as a data storage.

Kusto Query Language uses ***where*** tabular operator for filtering table data (e.g., StormEvents, Line 1) on conditions (Line 2). The condition consists of a Boolean expression for the table’s columns or predicate. The predicates can be “stacked” using Boolean “and” operator.

Suppose the result table should have selected columns or include, rename, drop, and insert computed columns. In that case, you need to use the ***project*** operator (Line 3) with the names of the selected or modified columns.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/az4-4.1.jpg)

Only these columns will be included in the result (Number 1).

![](https://s3.amazonaws.com/media.whizlabs.com/learn/az4-4.2.jpg)

Tabular operators in tabular expression statements are delimited by the pipe character (|). Each operator in a tabular statement takes input “from the pipe” — the result from previous pipe operation.

- **Options A is incorrect** because the tabular operator ***render*** instructs to present (generate) the result data in a particular way, e.g., visualize data as a chart, card, table (default), and interactive time pivot.
- **Options B is incorrect** because the tabular operator ***summarize*** aggregates the content of the input table for the output.
- **Options D is incorrect** because the operator ***let*** in the let statements binds a variable to a scalar or tabular expression.
- **Options E is incorrect** because the tabular operator ***find*** searches and finds the rows across a table set that matches a Boolean expression (predicate).
- **Options F is incorrect** because the tabular operator ***extend*** creates calculated columns and outputs them in the result set.
- **Options H is incorrect** because the operator ***set*** in the set statementsdeals with query options and their values.

For more information about Kusto Query Language tabular operators, please visit the below URLs:

- [https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/queries](https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/queries)
- [https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/whereoperator](https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/whereoperator)
- [https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/projectoperator](https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/projectoperator)

Question 15 Correct

**Domain:** Design and implement a source control strategy

Your team is working on an application with its code hosted in a git repository in Azure Repos. The application source is made up of multiple branches. You want to ensure that when the main branch is updated with the feature branch, it overrides the Git repository history. Which of the following would you use as a Git option for this?

- A. Rebase right
- B. Fetch
- C. Merge
- D. Push

###### Explanation:

Answer – A

For this, you can use the Rebase option. This just takes the commits on your branch and just replays them on an existing branch.

Option B is incorrect since this is used to fetch the latest changes.

Option C is incorrect since this is used for plain merging.

Option D is incorrect since this is used for pushing your changes onto the repository.

For more information on the rebase option, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/rebase?view=azure-devops&tabs=visual-studio](https://docs.microsoft.com/en-us/azure/devops/repos/git/rebase?view=azure-devops&tabs=visual-studio)

Question 16 Correct

**Domain:** Design and implement build and release pipelines

Your company currently has a set of applications deployed to Azure. All of the changes are managed via Azure DevOps. The requirements of each application, when it comes to feature releases, are given below.

| **Application Name** | **Requirement** |
| --- | --- |
| **whizlabapp1** | This is a mission critical application. You have to ensure that a small group of users first opt for testing changes to the application, before the actual change is released. |
| **whizlabapp2** | Here you need to minimize the deployment of changes to the application. You should be able to roll back also as quickly as possible. |

Which of the following is the release strategy you would opt for whizlabapp1?

- A. Blue/Green deployment
- B. Canary deployment right
- C. Rolling deployment
- D. Primary deployment

###### Explanation:

Answer - B

You can achieve this type of deployment with Canary deployments. Canary deployments are used to deploy changes to a set of users first. Once the users confirm that the application changes are fine, then the complete rollout can be carried out.

Option A is incorrect because this involves having two environments when it comes to application deployments.

Option C is incorrect because this involves making rolling deployments to infrastructure.

Option D is incorrect because this is not a valid deployment model.

For more information on an example on Canary deployments, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/virtual-machines/linux/tutorial-azure-devops-canary-strategy](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/tutorial-azure-devops-canary-strategy)

Question 17 Correct

**Domain:** Design and implement build and release pipelines

Your company currently has a set of applications deployed to Azure. All of the changes are managed via Azure DevOps. The requirements of each application, when it comes to feature releases, are given below.

| **Application Name** | **Requirement** |
| --- | --- |
| **whizlabapp1** | This is a mission critical application. You have to ensure that a small group of users first opt for testing changes to the application before the actual change is released |
| **whizlabapp2** | Here you need to minimize the deployment downtime. You should be able to roll back also as quickly as possible |

Which of the following is the release strategy you would opt for whizlabapp2?

- A. Blue/Green deployment right
- B. Canary deployment
- C. Rolling deployment
- D. Primary deployment

###### Explanation:

**Answer - A**

You can achieve this type of deployment with Blue/Green deployments. With this type of deployment, you can have two environments in place. When you are ready for the new version deployment, you can switch to the new environment. Then it allows you to switch back to the older environment at any point in time.

**Option B is incorrect** because this involves rolling out changes to a subset of users at a time.

**Option C is incorrect** because this involves making rolling deployments to infrastructure.

**Option D is incorrect** because this is not a valid deployment model.

For more information on an example of Blue/Green deployments, one can browse the following URL-

- [https://docs.microsoft.com/en-us/azure/virtual-machines/linux/tutorial-azure-devops-blue-green-strategy](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/tutorial-azure-devops-blue-green-strategy)

Question 18 Correct

**Domain:** Develop a security and compliance plan

A company's development team reports that adding new features to the application is taking longer due to technical debt.

You have to recommend changes that could help to reduce technical debt.

You recommend increasing the code duplication.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

Increasing code duplication will actually increase technical debt.

For more information on technical debt, one can browse to the following URL-

- [https://devblogs.microsoft.com/premier-developer/technical-debt-the-anti-devops-culture/](https://devblogs.microsoft.com/premier-developer/technical-debt-the-anti-devops-culture/)

Question 19 Correct

**Domain:** Develop a security and compliance plan

A company's development team reports that adding new features to the application is taking longer due to technical debt.  
You have to recommend changes that could help to reduce technical debt.  
You recommend increasing test coverage.  
Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

**Answer – A**

Creating unit tests as you develop code actually improves the code design and makes the code easier to understand by development teams in the future. As well as being more reliable, unit-tested code is simpler, more modular, and hence more reusable.

This reduces technical debt and lowers development costs in the long term. So improving code coverage helps in unit testing most of the code which in the long run reduces the technical debt.

For more information on technical debt, one can browse to the following URL-

- [https://devblogs.microsoft.com/premier-developer/technical-debt-the-anti-devops-culture/](https://devblogs.microsoft.com/premier-developer/technical-debt-the-anti-devops-culture/)
- [https://www.atlassian.com/agile/software-development/technical-debt](https://www.atlassian.com/agile/software-development/technical-debt)

Question 20 Correct

**Domain:** Develop a security and compliance plan

A company's development team reports that adding new features to the application is taking longer due to technical debt.  
You have to recommend changes that could help to reduce technical debt.  
You recommend refactoring the code.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

**Answer – A**

Yes, refactoring complex code can help in reducing technical debt.

For more information on technical debt, one can browse to the following URL-

- [https://devblogs.microsoft.com/premier-developer/technical-debt-the-anti-devops-culture/](https://devblogs.microsoft.com/premier-developer/technical-debt-the-anti-devops-culture/)

Question 21 Marked for review Incorrect

**Domain:** Develop a security and compliance plan

A company is planning to deploy a server application to an Azure virtual machine (VM). This will be running Windows Server 2019. The company also has an Azure Key Vault that stores secrets. You have to secure the key vault to secure API secrets for third-party integrations. Which of the following would you implement for this requirement?

- **Your Answer**
- A. Configure Role-based access control for the vault
- B. Change the application code to access the key vault
- E. Assign a Key Vault access role using Azure RBAC to the VM's managed identity
- **Correct Answer**
- B. Change the application code to access the key vault
- C. Implement a Key Vault access policy
- E. Assign a Key Vault access role using Azure RBAC to the VM's managed identity

###### Explanation:

**Correct Answers: B, C and E**

- **Change the application code to access the key vault**
- **Implement a Key Vault access policy**
- **Assign a Key Vault access role using Azure RBAC to the VM's managed identity**

And then change the application code to request access to the key vault via the managed identity.

Then, via Access policies, you will give access to the key vault for the virtual machine-managed identity.

System-assigned managed identities allow your Azure VM to securely authenticate to Azure services like Key Vault without storing credentials in your application code.

By assigning a Key Vault access role using Azure RBAC, you ensure that the VM has precise, auditable, and centrally managed permissions.  
This method aligns with Microsoft’s current best practices, which recommend using Azure RBAC over legacy access policies for managing Key Vault access.

- **Option A is incorrect because** you have to configure access policies for the key vault and not role-based access control.
- **Option D is incorrect because** you have to change the application code.

**Reference:**

- For more information on an example on using managed identities for an Azure virtual machine, one can browse to the following URL- [Tutorial - Use Azure Key Vault with a virtual machine in.NET | Microsoft Docs](https://docs.microsoft.com/en-us/azure/key-vault/general/tutorial-net-virtual-machine?tabs=azure-cli)

Question 22 Correct

**Domain:** Design and implement build and release pipelines

A company has an Azure subscription. They want to deploy a set of applications to a set of Azure virtual machines. Each application has different requirements when it comes to reliability.

| **Name** | **Requirement** |
| --- | --- |
| **whizlabapp1** | Be able to deploy the application across a set of identical virtual machines. The infrastructure should be able to meet demand automatically |
| **whizlabapp2** | Here the infrastructure needs to be available even in the event of a data center failure |

Which of the following would you recommend for whizlabapp1?

- A. Availability Sets
- B. Availability Zones
- C. Virtual Machine Scale Sets right
- D. Azure Traffic Manager

###### Explanation:

Answer – C

For this requirement, you can make use of Virtual Machine Scale Sets. With Virtual machine scale sets, the underlying virtual machines can scale out or in based on demand.

Options A and B are incorrect since this is used for managing the availability of virtual machines.

Option D is incorrect since this is a DNS routing-based service.

For more information on virtual machine scale sets, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview](https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview)

Question 23 Correct

**Domain:** Design and implement build and release pipelines

A company has an Azure subscription. They want to deploy a set of applications to a set of Azure virtual machines. Each application has different requirements when it comes to reliability.

| **Name** | **Requirement** |
| --- | --- |
| **whizlabapp1** | Be able to deploy the application across a set of identical virtual machines. The infrastructure should be able to meet demand automatically |
| **whizlabapp2** | Here the infrastructure needs to be available even in the event of a data center failure |

Which of the following would you recommend for whizlabapp2?

- A. Availability Sets
- B. Availability Zones right
- C. Virtual Machine Scale Sets
- D. Azure Traffic Manager

###### Explanation:

Answer – B

Option A is incorrect since Availability Sets can’t protect against data center level failures.

Option C is incorrect since this is used for scaling in and out virtual machines in your infrastructure.

Option D is incorrect since this is a DNS routing-based service.

For this requirement, you can make use of Availability Zones. Here you can protect your resources from an Azure Data Center failure.

For more information on Availability Zones, one can browse to the following URL-

- [https://docs.microsoft.com/en-us/azure/availability-zones/az-overview](https://docs.microsoft.com/en-us/azure/availability-zones/az-overview)

Question 24 Correct

**Domain:** Design and implement build and release pipelines

Your team has set up the following in their DevOps environment.

- An Azure DevOps project
- An Azure repo named “whizlabrepo” in the Azure DevOps project
- A Jenkins instance on an Azure virtual machine
- A project in Jenkins to carry out the build process for the application stored in Azure repo

You have to ensure that whenever a commit is made to Azure repo, it would trigger a build in Jenkins.

You create a build trigger in Jenkins.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

To accomplish the requirement of triggering a build in Jenkins whenever a commit is made to Azure Repos, you have to create a service hook in your Azure DevOps project.

For more information on creating a service hook in Azure DevOps, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/jenkins?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/jenkins?view=azure-devops)

Question 25 Correct

**Domain:** Design and implement build and release pipelines

Your team has set up the following in their DevOps environment.

- An Azure DevOps project
- An Azure repo named “whizlabrepo” in the Azure DevOps project
- A Jenkins instance on an Azure virtual machine
- A project in Jenkins to carry out the build process for the application stored in Azure repo

You have to ensure that whenever a commit is made to Azure repo, it would trigger a build in Jenkins.

You create a service hook in the Azure DevOps project.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

Answer – A

Yes, you can accomplish this by creating a service hook in Azure DevOps.

The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_25.png)

For more information on creating a service hook in Azure DevOps, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/jenkins?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/jenkins?view=azure-devops)

Question 26 Correct

**Domain:** Design and implement build and release pipelines

Your team has set up the following in their DevOps environment.

- An Azure DevOps project
- An Azure repo named “whizlabrepo” in the Azure DevOps project
- A Jenkins instance on an Azure virtual machine
- A project in Jenkins to carry out the build process for the application stored in Azure repo

You have to ensure that whenever a commit is made to Azure repo, it would trigger a build in Jenkins.

You create a service hook in Jenkins.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

The service hook needs to be created in Azure DevOps.

For more information on creating a service hook in Azure DevOps, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/jenkins?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/jenkins?view=azure-devops)

Question 27 Correct

**Domain:** Design and implement build and release pipelines

The following release pipeline has been defined in Azure DevOps.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_27-29.png)

The Artifacts section has been defined to pick up the artifacts from a build pipeline defined in Azure DevOps. The source code which is being build is an ASP.Net Core based solution. The application needs to be built on a Windows platform.

You have to ensure that the code released in the “Staging” stage is released to an Azure Web App instance named “whizlabstagingweb”. Where would you enable this setting?

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_27.1.png)

- A. In the (1) Stages section
- B. In the (2) pre-conditions section
- C. In the (3) job/task section right
- D. In the (4) post-condition section

###### Explanation:

Answer – C

You can implement this in the job/task section. If you go to this section, you can add a task of “Deploy Azure App Service”.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_27.2.png)

Here you can define the App Service Type as “Web App on Windows”. And then, you can define the App Service name.

Since this is clear from the implementation, all other options are incorrect.

For more information on build and release tasks, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/process/tasks?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/tasks?view=azure-devops&tabs=yaml)

Question 28 Correct

**Domain:** Design and implement build and release pipelines

The following release pipeline has been defined in Azure DevOps.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_27-29_01_27.png)

The Artifacts section has been defined to pick up the artifacts from a build pipeline defined in Azure DevOps. The source code which is being build is an ASP.Net Core based solution. The application needs to be built on a Windows platform.

You have to ensure that the code released in the “Production” stage is released to an Azure Web App instance named “whizlabproductionweb”. Where would you enable this setting?

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_28.1.png)

- A. In the (1) Stages section
- B. In the (2) pre-conditions section
- C. In the (3) job/task section right
- D. In the (4) post-condition section

###### Explanation:

Answer – C

You can implement this in the job/task section. If you go to this section, you can add a task of “Deploy Azure App Service”.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_28.2.png)

Here you can define the App Service Type as “Web App on Windows”. And then, you can define the App Service name.

Since this is clear from the implementation, all other options are incorrect.

For more information on build and release tasks, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/process/tasks?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/tasks?view=azure-devops&tabs=yaml)

Question 29 Correct

**Domain:** Design and implement build and release pipelines

The following release pipeline has been defined in Azure DevOps.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_27-29_01_43.png)

The Artifacts section has been defined to pick up the artifacts from a build pipeline defined in Azure DevOps. The source code which is being build is an ASP.Net Core based solution. The application needs to be built on a Windows platform.

You need to define the number of days a release can be retained. Where would you define this?

- A. In the Tasks section
- B. In the Variables section
- C. In the Retention section right
- D. In the Options section

###### Explanation:

Answer – C

You would define this in the Retention section, as shown below.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_29.1.png)

The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_29.2.png)

Since this is clear from the implementation, all other options are incorrect.

For more information on retention policies, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/policies/retention?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/policies/retention?view=azure-devops)

Question 30 Correct

**Domain:** Design and implement a source control strategy

A company wants to start using the Azure DevOps tools. They have set up an organization and a project. They want to set up multiple Azure repositories. Different project teams would use each repository.

Each project team has different requirements for the source code versioning system, as given below.

| **Project team** | **Requirement** |
| --- | --- |
| **TeamA** | Developers should be able to create branches to work on. They should be able to see file history on their local machines |
| **TeamB** | Developers should be able to apply permissions at the file level. |
| **TeamC** | Developers should be able to use the source code versioning system from third-party Integrated development environments |

Which of the following would you recommend as the source code versioning system to use in Azure Repos for TeamA?

- A. Team Foundation Version Control
- B. Git right
- C. Subversion
- D. Perforce

###### Explanation:

Answer – B

You can accomplish this using Git in Azure Repos.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_30.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on using Git vs Team Foundation version control, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/tfvc/comparison-git-tfvc?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/tfvc/comparison-git-tfvc?view=azure-devops)

Question 31 Correct

**Domain:** Design and implement a source control strategy

A company wants to start using the Azure DevOps tools. They have set up an organization and a project. They want to set up multiple Azure repositories. Different project teams would use each repository.

Each project team has different requirements for the source code versioning system, as given below.

| **Project team** | **Requirement** |
| --- | --- |
| **TeamA** | Developers should be able to create branches to work on. They should be able to see file history on their local machines |
| **TeamB** | Developers should be able to apply permissions at the file level. |
| **TeamC** | Developers should be able to use the source code versioning system from third-party Integrated development environments |

Which of the following would you recommend as the source code versioning system to use in Azure Repos for TeamB?

- A. Team Foundation Version Control right
- B. Git
- C. Subversion
- D. Perforce

###### Explanation:

**Answer – A**

You can accomplish this using Team Foundation Version Control in Azure Repos.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_31.png)

**Option B is incorrect** because Git supports permissions only at the branch or repository level.

**Option C is incorrect** because Subversion is not supported by Azure Repository.

**Option D is incorrect** because Perforce is not supported by Azure Repository.

For more information on using Git vs Team Foundation version control, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/tfvc/comparison-git-tfvc?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/tfvc/comparison-git-tfvc?view=azure-devops)

Question 32 Marked for review Incorrect

**Domain:** Design and implement a source control strategy

A company wants to start using the Azure DevOps tools. They have set up an organization and a project. They want to set up multiple Azure repositories. Different project teams would use each repository.  
Each project team has different requirements for the source code versioning system, as given below.

| **Project team** | **Requirement** |
| --- | --- |
| **TeamA** | Developers should be able to create branches to work on. They should be able to see file history on their local machines |
| **TeamB** | Developers should be able to apply permissions at the file level. |
| **TeamC** | Developers should be able to use the source code versioning system from third-party Integrated development environments |

Which of the following would you recommend as the source code versioning system to use in Azure Repos for TeamC?

- A. Team Foundation Version Control right
- B. Git right
- C. Subversion wrong
- D. Perforce

###### Explanation:

**Answer – A and B**

There are two correct answers TFVC and Git.  
You can accomplish this using Git in Azure Repos.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/28/ckeditor_32.png)

**Option C is incorrect** because Subversion is not supported by Azure Repository.

**Option D is incorrect** because Perforce is not supported by Azure Repository.

For more information on using Git vs Team Foundation version control, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/tfvc/comparison-git-tfvc?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/tfvc/comparison-git-tfvc?view=azure-devops)

Question 33 Marked for review Correct

**Domain:** Define and implement continuous integration

You have to create a multi-stage docker image for an ASP.Net core 2.2 application. Below is the incomplete Dockerfile. The Dockerfile is located in your project directory.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_33-36.png)

Which of the following would go into Slot 1?

- A. mcr.microsoft.com/dotnet/core/aspnet:2.2
- B. mcr.microsoft.com/dotnet/sdk:6.0 right
- C. ENTRYPOINT
- D. RUN
- E. FROM

###### Explanation:

**Answer – B**

The first stage of the Dockerfile is to go ahead and build the.Net application. For this, we need to use the.net core SDK.

An example of this is given in the Docker documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/DockerFile.PNG)

**Option A is incorrect** because it's not the correct image for this requirement.

**Option C is incorrect** because we need the image name and not the command.

**Option D is incorrect** because we need the image name and not the command.

**Option E is incorrect** because we need the image name and not the command.

**Reference:** For more information on creating Dockerfile for.net core applications, please visit the below URL-

- [Containerize an app with Docker tutorial -.NET | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/core/docker/build-container?tabs=windows)

Question 34 Correct

**Domain:** Design and implement build and release pipelines

You have to create a multi-stage docker image for an ASP.Net core 2.2 application. Below is the incomplete Dockerfile. The Dockerfile is located in your project directory.

![](https://www.whizlabs.com/learn/media/2020/08/31/ckeditor_33-36_39_28.png)

Which of the following would go into Slot2?

- A. mcr.microsoft.com/dotnet/core/aspnet:2.2
- B. mcr.microsoft.com/dotnet/core/sdk:2.2
- C. ENTRYPOINT
- D. RUN right
- E. FROM

###### Explanation:

Answer – D

The next part is to use the “RUN” command to publish a release of the application.

An example of this is given in the Docker documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_34.png)

Since this is clearly given in the Docker documentation, all other options are incorrect.

**Reference**: For more information on creating Dockerfile for.net core applications, please visit the below URL-

- [Containerize an app with Docker tutorial -.NET | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/core/docker/build-container?tabs=windows)

Question 35 Correct

**Domain:** Design and implement build and release pipelines

You have to create a multi-stage docker image for an ASP.Net core 2.2 application. Below is the incomplete Dockerfile. The Dockerfile is located in your project directory.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_33-36_49_06.png)

Which of the following would go into Slot3?

- A. mcr.microsoft.com/dotnet/aspnet:6.0 right
- B. mcr.microsoft.com/dotnet/core/sdk:2.2
- C. ENTRYPOINT
- D. RUN
- E. FROM

###### Explanation:

**Answer – A**

Now we need to use the runtime image to run the application.  
An example of this is given in the Docker documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/Docker2.PNG)

**Option B is incorrect** because it's not the correct image for this command.

**Option C is incorrect** because we need the image name and not the command.

**Option D is incorrect** because we need the image name and not the command.

**Option E is incorrect** because we need the image name and not the command.

For more information on creating Dockerfile for.net core applications, please visit the below URL-

- [Dockerize an ASP.NET Core application | Docker Documentation](https://docs.docker.com/samples/dotnetcore/)

Question 36 Correct

**Domain:** Design and implement build and release pipelines

You have to create a multi-stage docker image for an ASP.Net core 2.2 application. Below is the incomplete Dockerfile. The Dockerfile is located in your project directory.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_33-36_48_58.png)

Which of the following would go into Slot4?

- A. mcr.microsoft.com/dotnet/core/aspnet:2.2
- B. mcr.microsoft.com/dotnet/core/sdk:2.2
- C. ENTRYPOINT right
- D. RUN
- E. FROM

###### Explanation:

Answer – C

Finally, we use the “ENTRYPOINT” clause to specify the “dll” that needs to run our application.

An example of this is given in the Docker documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_36.png)

Since this is clearly given in the Docker documentation, all other options are incorrect.

For more information on creating Dockerfile for.net core applications, please visit the below URL-

- [https://docs.docker.com/engine/examples/dotnetcore/](https://docs.docker.com/engine/examples/dotnetcore/)

Question 37 Correct

**Domain:** Develop a security and compliance plan

You are configuring a pipeline in Azure DevOps that builds and deploys a Node.js application. You want to ensure that all code commits are scanned for secrets like API keys before being integrated into the pipeline.

What should you integrate into the pipeline to meet this requirement?

- A. Microsoft Defender for Cloud
- B. Azure Key Vault
- C. GitHub Advanced Security right
- D. Azure DevOps secret scanning

###### Explanation:

**Correct Answer: C**

- **Option C is CORRECT** because GitHub Advanced Security provides built-in capabilities to scan code repositories for security vulnerabilities, including secrets like API keys. It integrates directly with GitHub repositories and can scan code commits in real time to identify and alert on potential security issues, including exposed secrets. By integrating GitHub Advanced Security into your Azure DevOps pipeline, you can ensure that all code changes are automatically scanned for secrets before being integrated into the pipeline.
- **Option A is INCORRECT** because Microsoft Defender for Cloud primarily focuses on security posture management and threat protection across Azure services and hybrid workloads. While it provides security recommendations and alerts, it does not offer specific capabilities to scan code commits for secrets like API keys. It is more suitable for monitoring and securing Azure infrastructure and services rather than code-level secrets.
- **Option B is INCORRECT** because Azure Key Vault functions as a secure storage service designed for managing and protecting cryptographic keys, secrets, and certificates. While it offers centralized access control for secrets, its purpose revolves around securely storing and retrieving secrets used by applications and services, rather than actively scanning code repositories for potential secrets.
- **Option D is INCORRECT** because Azure DevOps does not have a built-in feature called "secret scanning." While Azure DevOps provides capabilities for the secure handling of secrets through variable groups and Azure Key Vault integration, it does not inherently scan code commits for secrets like API keys. Its focus is on build, test, and release automation rather than code scanning for security vulnerabilities or secrets.

**Reference:**

- [https://learn.microsoft.com/en-gb/azure/devops/repos/security/github-advanced-security-secret-scanning?view=azure-devops](https://learn.microsoft.com/en-gb/azure/devops/repos/security/github-advanced-security-secret-scanning?view=azure-devops)

Question 38 Correct

**Domain:** Implement an instrumentation strategy

Contoso's development team relies on prompt notifications for any critical issues that arise in their environments. You configure Azure Monitor to ensure that alerts are sent to your DevOps team via both email and SMS.

Solution: You set up an Action Group within Azure Monitor and include the necessary email addresses and phone numbers for the team members.

Does the solution meet the objective? \[Select Yes/No\]

- A. Yes right
- B. No

###### Explanation:

**Correct Answer: A**

- **Option A is CORRECT** because configuring an Action Group within Azure Monitor is the standard method to notify team members via email and SMS. Action Groups are designed to define a set of recipients and notification methods for alerts generated by Azure Monitor. By including the necessary email addresses and phone numbers in the Action Group, you ensure that the specified contacts receive notifications through their preferred communication channels (email and SMS). This setup is effective for ensuring that the DevOps team is promptly informed of any critical issues, allowing them to respond quickly.
- **Option B is INCORRECT** because the described setup in the Action Group is the appropriate method for achieving notifications through email and SMS within Azure Monitor.

**References:**

- [https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/action-groups](https://learn.microsoft.com/en-us/azure/azure-monitor/alerts/action-groups)

Question 39 Correct

**Domain:** Design and implement build and release pipelines

A company wants to implement DevOps processes for a set of applications. These applications are based on the.Net framework. They want to ensure that security validation is performed during each stage of the application lifecycle. They want to ensure the following.

- Static Code Analysis is performed during the development stage.
- Static Code Analysis is performed during the Continuous Integration stage.
- All high severity issues are logged in a tracking tool.

You have to advise on the right tool that can be used for these requirements.

Which of the following can be used for the requirement?

**“Static Code Analysis is performed during the Continuous Integration stage”.**

- A. Slack
- B. Jenkins
- C. SonarQube right
- D. PMD
- E. Azure Boards

###### Explanation:

Answer – C

SonarQube is a code analysis tool that can be used during the development and continuous integration stage.

Below is a snippet from the SonarQube documentation on what you can achieve with the tool.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_38.png)

Option A is incorrect since this is a collaboration-based tool.

Option B is incorrect since this is a continuous integration tool.

Option D is incorrect since this tool can be used for Java-based applications only.

Option E is incorrect since this tool is used for managing software projects.

For more information on SonarQube, please visit the below URL-

- [https://www.sonarqube.org/](https://www.sonarqube.org/)

Question 40 Correct

**Domain:** Design and implement processes and communications

A company currently has an organization and project defined in Azure DevOps services. For one of the projects, the company wants to gather feedback from users related to certain work items for a particular release. You have to ensure the following.

- The release team can request feedback from users.
- Users have the ability to provide feedback for the work items.
- Users have the required tools installed for giving feedback.

You have to ensure that licensing cost is kept to a minimum.

What should be installed for the users to give feedback for the work items?

- A. The Azure DevOps extension
- B. The Team Foundation extension
- C. The Test & Feedback extension right
- D. The Test extension

###### Explanation:

Answer – C

You have to use the Test & Feedback extension.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_40.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on providing feedback, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/project/feedback/get-feedback?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/project/feedback/get-feedback?view=azure-devops)

Question 41 Incorrect

**Domain:** Implement an instrumentation strategy

You are responsible for monitoring the performance and availability of multiple Azure virtual machines in your organization. Your goal is to collect detailed metrics on CPU usage, memory consumption, and disk performance to ensure the virtual machines are operating efficiently and to identify any potential issues.

Solution: You configure Azure Monitor Application Insights on each virtual machine.

Does the solution meet the objective? \[Select Yes/No\]

- A. Yes wrong
- B. No right

###### Explanation:

**Correct Answer: B**

- **Option B is CORRECT** because, for the aforementioned scenario, we need VM Insights and not Application Insights. Azure Monitor VM Insights is specifically designed to monitor the performance and health of virtual machines. VM Insights collects and analyzes data such as CPU usage, memory usage, disk performance, and network traffic. It provides in-depth insights into the operational status of virtual machines, helping administrators troubleshoot issues, optimize performance, and ensure availability. VM Insights leverages the Azure Monitor agent to gather this data and present it in an easily consumable format within the Azure portal.
- **Option A is INCORRECT** because Azure Application Insights is primarily designed for monitoring the performance, availability, and usage patterns of web applications. It provides telemetry data such as request rates, response times, dependency tracking, and exception reports, which are essential for understanding how an application is performing from an end-user perspective. However, it does not provide detailed performance metrics specifically for virtual machines such as CPU, memory, and disk usage.

**Reference:**

- [https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-overview](https://learn.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-overview)

Question 42 Correct

**Domain:** Develop a security and compliance plan

A company is currently looking at implementing a set of tools for developing and deploying applications. The applications would run through a DevOps cycle for all change requests. The company wants to ensure that the right tool is in place for scanning the application for any open-source package security vulnerabilities.

They decide to use the Jenkins application for this requirement.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

This is a tool used for Continuous Integration.

For more information on Jenkins, please visit the below URL-

- [https://jenkins.io/](https://jenkins.io/)

Question 43 Correct

**Domain:** Develop a security and compliance plan

A company is currently looking at implementing a set of tools for developing and deploying applications. The applications would run through a DevOps cycle for all change requests. The company wants to ensure that the right tool is in place for scanning the application for any open-source package security vulnerabilities.

They decide to use the BlackDuck by Synopsys application for this requirement.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

Answer – A

Yes, this tool will accomplish the requirement.

The Azure Marketplace mentions the following on this tool.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_43.png)

For more information on the tool, please visit the below URL-

- [https://azuremarketplace.microsoft.com/en-us/marketplace/apps/black-duck-software.blackduck\_hub\_431](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/black-duck-software.blackduck_hub_431)

Question 44 Correct

**Domain:** Design and implement build and release pipelines

A team needs to automate the User Interface testing for a web application. They also need to integrate the testing of the application in the build lifecycle of the application. Which of the following could they use for this purpose?

- A. SonarQube
- B. XUnit
- C. Selenium right
- D. Microsoft.CodeAnalysis

###### Explanation:

Answer – C

The right tool to use for User Interface testing is Selenium.

The Microsoft documentation also has an article on this.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_44.png)

Option A is incorrect since this tool is used to check for application vulnerabilities.

Option B is incorrect since this tool is used for Unit testing.

Option D is incorrect since this tool is used for code Analysis.

For more information on working with Selenium, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/test/continuous-test-selenium?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/test/continuous-test-selenium?view=azure-devops)

Question 45 Correct

**Domain:** Design and implement build and release pipelines

A team is currently creating resource manager templates for building virtual machines on Azure. They have to use the Azure Key Vault service for storing the virtual machine account password. A Key Vault has been created and secrets created in the service.

The following parameter file is being created to recover the secret from the Key Vault.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_45-47_10_49.png)

Which of the following would go into Slot2?

- A. “secretName”
- B. “password”
- C. “keyVault”
- D. “id” right

###### Explanation:

Answer – D

Here we have to mention the reference as “id”.

An example is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_46.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on working with secrets in resource manager templates, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-manager-keyvault-parameter](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-manager-keyvault-parameter)

Question 46 Correct

**Domain:** Design and implement build and release pipelines

A team is currently creating resource manager templates for building virtual machines on Azure. They have to use the Azure Key Vault service for storing the virtual machine account password. A Key Vault has been created and secrets created in the service.

The following parameter file is being created to recover the secret from the Key Vault.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_45-47.png)

Which of the following would go into Slot1?

- A. “secretName”
- B. “password”
- C. “keyVault” right
- D. “id”

###### Explanation:

Answer – C

Here we have to mention the reference as “keyVault”.

An example is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_45.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on working with secrets in resource manager templates, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-manager-keyvault-parameter](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-manager-keyvault-parameter)

Question 47 Correct

**Domain:** Design and implement build and release pipelines

A team is currently creating resource manager templates for building virtual machines on Azure. They have to use the Azure Key Vault service for storing the virtual machine account password. A Key Vault has been created and secrets created in the service.

The following parameter file is being created to recover the secret from the Key Vault.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_45-47_10_55.png)

Which of the following would go into Slot3?

- A. “secretName” right
- B. “password”
- C. “keyVault”
- D. “id”

###### Explanation:

Answer – A

Here we have to mention the “secretName”.

An example is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_47.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on working with secrets in resource manager templates, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-manager-keyvault-parameter](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-manager-keyvault-parameter)

Question 48 Marked for review Correct

**Domain:** Implement an instrumentation strategy

You have the following query that presents a pie chart of virtual machine processes contributing to the CPU Utilization and aggregated at a granularity of 1 min.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/PT-5-Q48.1.png)

What are the three operators used in this query?

- **Your Answer**
- 1.
	E. where
- 2.
	D. summarize
- 3.
	B. render
- **Correct Answer**
- 1.
	E. where
- 2.
	D. summarize
- 3.
	B. render

###### Explanation:

**Correct Answer:** **E, D and B**

- **where**
- **summarize**
- **render**
- **A is incorrect** **because the operator** ***let*** **in the let statements binds a variable to a scalar or tabular expression.**
- **B is correct because** to present the data, Kusto Query Language(KQL) provides tabular operator **render***.*
- **C is incorrect because the tabular operator *extend* creates calculated columns and outputs them in the result set.**
- **D is correct because** To aggregate the input data and present it in the output table, need to use a tabular operator **Summarize**
- **E is correct because** Kusto Query Language(KQL) uses **where** tabular operator for table data.

Microsoft Azure Monitor stores two types of data: logs and metrics. This data helps users monitor, tune, and troubleshoot their applications and services. Azure Monitor collects data from applications, operating systems, Azure resources, subscriptions, tenants, and custom sources.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/PT-5-Q48.png)

Kusto Query Language uses **where** tabular operator for filtering table data (e.g., Perf, Line 1) on conditions (Line 2 - 4). The condition consists of a Boolean expression for the table’s columns or predicate. The predicates are “stacked” using Boolean “and” operator (Line 3 - 4).

To aggregate the input data and present it in the output table, you need to use a tabular operator **summarize** (Line 5).

To present the data, KQL provides a tabular operator **render***.* This operator generates the result data in a particular way, e.g., visualize data as a chart (e.g., piechart (Line 6)), card, table (default), and interactive time pivot. The render should always be the last operator in tabular expression.

**References:**

- [Tutorial: Kusto queries | Microsoft Docs](https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/tutorial?pivots=azuredataexplorer)
- [Examine Kusto Query Language (KQL) - Learn | Microsoft Docs](https://docs.microsoft.com/en-us/learn/modules/implement-tools-track-usage-flow/5-examine-kusto-query-language-kql)

Question 49 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

A Kubernetes cluster has just been setup. Which of the following command could be used to get the status of the nodes in the cluster?

- A. az aks get nodes
- B. kubectl get nodes right
- C. az get nodes
- D. docker get nodes

###### Explanation:

Answer – B

This can be down with the help of the “kubectl” command.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_49.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on creating and working with Kubernetes clusters, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/aks/kubernetes-walkthrough-rm-template](https://docs.microsoft.com/en-us/azure/aks/kubernetes-walkthrough-rm-template)

Question 50 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

You need to ensure that Azure build pipelines can connect to the on-premise GitHub Enterprise Server. Which of the following would you create for this requirement?

- A. A service connection in the project in Azure DevOps services right
- B. A service connection in the organization in Azure DevOps services
- C. A service hook in the project in Azure DevOps services
- D. A service hook in the organization in Azure DevOps services

###### Explanation:

**Answer – A**

You need to create a service connection as shown below.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_50.png)

Since this is clear from the implementation, all other options are incorrect.

For more information on service connections, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github-enterprise?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github-enterprise?view=azure-devops)
- [https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)

Question 51 Incorrect

**Domain:** Design and implement processes and communications View Case Study  

You need to allocate the right process template in Azure Boards.

You decide to use the “Agile” process template.

Would this fulfill the requirement?

- A. Yes wrong
- B. No right

###### Explanation:

Answer – B

This template does not contain the definitions for change or review requests.

For more information on process templates, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&tabs=basic-process](https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&tabs=basic-process)

Question 52 Correct

**Domain:** Design and implement processes and communications View Case Study  

You need to allocate the right process template in Azure Boards.

You decide to use the “Scrum” process template.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

This template does not contain the definitions for change or review requests.

For more information on process templates, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&tabs=basic-process](https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&tabs=basic-process)

Question 53 Correct

**Domain:** Design and implement processes and communications View Case Study  

You need to allocate the right process template in Azure Boards.

You decide to use the “CMMI” process template.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

Answer – A

Yes, this process template has the work items for change and review requests.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_53.png)

For more information on process templates, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&tabs=basic-process](https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&tabs=basic-process)

Question 54 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

You need to ensure that when Resource Manager templates are deployed, the Resource Manager leaves unchanged resources that exist in the resource group that aren’t specified in the template. Which of the following mode in the template should be used to accomplish this requirement?

- A. Complete
- B. Nested
- C. Incremental right
- D. Linked

###### Explanation:

Answer – C

You need to specify the Incremental mode.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_54.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on template deployment modes, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/azure-resource-manager/deployment-modes](https://docs.microsoft.com/en-us/azure/azure-resource-manager/deployment-modes)

Question 55 Correct

**Domain:** Design and implement processes and communications View Case Study  

The management wants to see a chart to understand whether the teams are able to complete the work allocated to a sprint. The chart should be calibrated against the work items. Which of the following would you use as the widget to use in Azure Boards for this requirement?

- A. Velocity right
- B. Cycle Time
- C. Lead Time
- D. Burn Down

###### Explanation:

Answer – A

This can be accomplished with the “Velocity” widget.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/31/ckeditor_55.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

For more information on widgets in Azure Boards, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/report/dashboards/analytics-widgets?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/report/dashboards/analytics-widgets?view=azure-devops)