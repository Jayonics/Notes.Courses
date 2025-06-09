---
title: "LMS | Whizlabs"
source: "https://www.whizlabs.com/learn/course/microsoft-azure-certification-az-400/270/quiz/18784/report/8328981"
author:
published:
created: 2025-05-29
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
| 1 | Develop a security and compliance plan | 12 | 11 | 1 | 0 | 3 |
| 2 | Design and implement a source control strategy | 9 | 7 | 2 | 0 | 3 |
| 3 | Design and implement build and release pipelines | 15 | 12 | 3 | 0 | 2 |
| 4 | Implement an instrumentation strategy | 12 | 9 | 3 | 0 | 3 |
| 5 | Design and implement processes and communications | 7 | 6 | 1 | 0 | 1 |
| Total | All Domains | 55 | 45 | 10 | 0 | 12 |

Question 1 Marked for review Incorrect

**Domain:** Design and implement a source control strategy

Your team is automating the build process for a Java-based application by using Azure DevOps. The team needs to calculate the code coverage and then publish the results in Azure Pipeline. Which of the following can be used for calculating the code coverage?

- A. DevTest
- B. MSTest wrong
- C. Cobertura right
- D. JavaTest

###### Explanation:

**Correct Answer - C**

**Explanation:** Cobertura is a code coverage tool for Java. Below is a snippet of the documentation page for the tool.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/25/ckeditor_1.1.png)

It also can publish results to Azure DevOps as mentioned in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/25/ckeditor_1.2.png)

**Option A is incorrect** because DevTest is not a code coverage tool, it's an approach in software development that aims to bring the development and testing phases closer together.

**Option B is incorrect** because MSTest is a Unit testing framework for the.NET framework.

**Option C is CORRECT** because Cobertura is a Java code coverage reporting tool.

**Option D is incorrect** because JavaTest is a Regression testing framework, not a code coverage tool.

For more information on the code coverage tool and publishing results, please visit the below URL-

- [http://cobertura.github.io/cobertura/](http://cobertura.github.io/cobertura/)
- [https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/test/publish-code-coverage-results?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/test/publish-code-coverage-results?view=azure-devops)

Question 2 Marked for review Correct

**Domain:** Design and implement build and release pipelines

A team is planning to use Azure Automation for a set of Azure Virtual machines. They need to use Azure state configuration to manage the state of the virtual machines. Which of the following actions would be needed to ensure the performance and state of the virtual machines effectively? (Select all the steps that are applicable)

- **Your Answer**
- A. Onboard the set of virtual machines onto Azure Automation
- E. Compile the configuration
- F. Upload a configuration
- C. Assign the node configuration
- B. Check the status of the node
- **Correct Answer**
- A. Onboard the set of virtual machines onto Azure Automation
- F. Upload a configuration
- E. Compile the configuration
- C. Assign the node configuration
- B. Check the status of the node

###### Explanation:

**Correct Answer: A, F, E, C, and B**

- **Onboard the set of virtual machines onto Azure Automation**
- **Upload a configuration**
- **Compile the configuration**
- **Assign the node configuration**
- **Check the status of the node**
- **Options A, F, E, C, and B are correct** for configuring machines to a desired state as per the Microsoft documentation

![](https://s3.amazonaws.com/media.whizlabs.com/learn/PT-1-Q2.png)

- **Option D is incorrect** as it's required in Azure Kubernetes Service for node pool and not in Azure Automation State Configuration.
- **Option G is incorrect** as tags are key-value pairs that help you identify resources based on settings that are relevant to your organization, and this is not required for Azure Automation State Configuration.

**Reference:**

- For more information on Azure Automation State Node configuration, please visit the below URL - [Get started with Azure Automation State Configuration | Microsoft Docs](https://docs.microsoft.com/en-us/azure/automation/automation-dsc-getting-started)

Question 3 Correct

**Domain:** Develop a security and compliance plan

A team is using Azure Resource Manager templates in their DevOps pipeline. The templates need to refer to secrets in the Azure Key Vault dynamically. You must complete the below snippet of the Resource Manager template.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/25/ckeditor_3.png)

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/25/ckeditor_3.1.png)

Which of the following would go into Slot1?

- A. Microsoft.Deployments/resources
- B. Deployments.Resources
- C. Microsoft.Resources/deployments right
- D. Resources/Azure.KeyVault

###### Explanation:

**Correct Answer – C**

An example of this is given in the Microsoft documentation on an ARM template. This is used to refer to secrets dynamically from an Azure Key Vault service.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/25/ckeditor_3.4.png)

The Sample Template is as follows

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/11/19/ckeditor_111.png)

**Option A is incorrect** as "Microsoft.Deployments/resources" is not the correct syntax.

**Option B is incorrect** as "Deployments.Resources" is not the correct syntax.

**Option C is CORRECT** as the syntax is a valid syntax as per Microsoft documentation.

**Option D is incorrect** as "Resources/Azure.KeyVault" is not the correct syntax.

For more information on referencing the Azure Key Vault in the Resource Manager, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/templates/microsoft.resources/deployments#template-format](https://docs.microsoft.com/en-us/azure/templates/microsoft.resources/deployments#template-format)

Question 4 Marked for review Incorrect

**Domain:** Develop a security and compliance plan

A team is using Azure Resource Manager templates in their DevOps pipeline. The templates need to refer to secrets in the Azure Key vault dynamically. You need to complete the below snippet of the Resource Manager template.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_4.1.png)

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_4.2.png)

Which of the following would go into Slot2?

- A. templateURI wrong
- B. templateLink right
- C. keyVaultlink
- D. secretlink

###### Explanation:

**Answer – B**

An example of this is given in the Microsoft documentation on an ARM template. This is used to refer to secrets dynamically from an Azure Key Vault service.

.![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/11/19/ckeditor_111.png)

Since this is clearly given in the Microsoft documentation, all other options are incorrect.

**Option A is incorrect** as templateURI is used in PowerShell script for deployment and not in an ARM template.

**Option B is CORRECT** as templateLink is a correct property as per Microsoft documentation.

**Option C is incorrect** as the kyeVaultlink is not an ARM templates property.

**Option D is incorrect** as secretlink is not an ARM template property.

For more information on referencing the Azure Key Vault in the Resource Manager, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/templates/microsoft.resources/deployments#template-format](https://docs.microsoft.com/en-us/azure/templates/microsoft.resources/deployments#template-format)

Question 5 Correct

**Domain:** Develop a security and compliance plan

A team is currently working on a Java-based project in an Azure DevOps environment. A solution needs to be recommended to improve the quality of code within the DevOps project.  
Which of the following would you recommend?

- A. For a Maven build task, enable CheckStyle
- B. For a Maven build task, enable Run PMD and Run CheckStyle right
- C. For a Gradle build task, enable CheckStyle.
- D. For an ANT build task, enable FindBugs.

###### Explanation:

**Answer – B**

PMD is a source code analyzer. It finds common programming flaws like unused variables, empty catch blocks, unnecessary object creation, and so forth.

Checkstyle is a development tool to help programmers write Java code that adheres to a coding standard.

Below is a snippet contains a short introduction to PMD tool:

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_5.1.png)

In Azure DevOps, you can enable this as shown in the Microsoft documentation below.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_5.2.png)

**Option A is incorrect** as this tool is only used for style checks.

**Option B is CORRECT** as both tools in combination (PMD and CheckStyle) help to improve the code quality.

**Option C is incorrect** as this tool is only used for style checks.

**Option D is incorrect** as you need to use either a Maven or Gradle build task.

For more information on PMD and enabling it for a Java project, please visit the below URL-

- [https://pmd.github.io/](https://pmd.github.io/)
- [https://devblogs.microsoft.com/devops/the-maven-build-task-now-supports-pmd-analysis-out-of-the-box/](https://docs.microsoft.com/en-us/azure/devops/java/standalone-tools?view=azure-devops)
- [https://devblogs.microsoft.com/devops/gradle-build-task-supports-checkstyle-analysis/](https://devblogs.microsoft.com/devops/gradle-build-task-supports-checkstyle-analysis/)

Question 6 Correct

**Domain:** Develop a security and compliance plan

A team is currently building and deploying an application using Azure DevOps services. You have to use the right security tool during the following phase of the development lifecycle.

- After a pull request
- During the continuous integration phase
- During the continuous delivery phase

Which of the following would you use for the pull request phase?

- A. Static Code Analysis right
- B. Penetration Testing
- C. Threat Modeling
- D. Load Testing

###### Explanation:

**Correct Answer – A**

During the coding phase, it is always preferential to use static code analysis tools. The Microsoft documentation mentions the following.

![](https://media.whizlabs.com/website/378813160_1695385089.png)

**Option A is CORRECT since static code analysis is performed once the pull request is raised.**

**Option B is incorrect** since Penetration Testing should be used during the deployment phase.

**Option C is incorrect** since the Threat Modeling tool should be used during the design phase.

**Option D is incorrect** since Load Testing should be used during the deployment phase.

**References:**

- [Azure Pipelines architecture for Azure Web Apps - Azure Pipelines | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/pipelines/architectures/devops-pipelines-azure-web-apps-architecture?view=azure-devops#architecture)
- [What is DevOps? - Azure DevOps | Microsoft Learn](https://learn.microsoft.com/en-us/devops/what-is-devops#devops-and-the-application-lifecycle)
- [DevSecOps: bringing security into your DevOps practice on Azure | Microsoft Learn](https://learn.microsoft.com/en-us/shows/azure-enablement/devsecops-bringing-security-into-your-devops-practice-on-azure)

Question 7 Marked for review Correct

**Domain:** Develop a security and compliance plan

A team is currently building and deploying an application using Azure DevOps services. You have to use the right security tool during the following phase of the development lifecycle.

- After a pull request
- During the continuous integration phase
- During the continuous delivery phase

Which of the following would you use for the continuous integration phase?

- A. Penetration Testing
- B. Threat Modeling
- C. Static Code Analysis right
- D. Load Testing

###### Explanation:

**Correct Answer – C**

During the CI phase, it is always preferential to use static code analysis tools. The Microsoft documentation mentions the following.

![](https://media.whizlabs.com/website/167628596_1695384884.png)

**Option A is incorrect** since Penetration Testing should be used during the deployment phase.

**Option B is incorrect** since the Threat Modeling tool should be used during the design phase.

**Option C is CORRECT since in this phase code is merged in the master/main branch and is yet to be deployed, so it can be scanned for any quality issues or security issues in code before going for deployment and it's as per Microsoft's recommendation as well.**

**Option D is incorrect** since the Load Testing tool should be used during the deployment phase.

**References:**

- [Azure Pipelines architecture for Azure Web Apps - Azure Pipelines | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/pipelines/architectures/devops-pipelines-azure-web-apps-architecture?view=azure-devops#architecture)
- [What is DevOps? - Azure DevOps | Microsoft Learn](https://learn.microsoft.com/en-us/devops/what-is-devops#devops-and-the-application-lifecycle)
- [DevSecOps: bringing security into your DevOps practice on Azure | Microsoft Learn](https://learn.microsoft.com/en-us/shows/azure-enablement/devsecops-bringing-security-into-your-devops-practice-on-azure)

Question 8 Marked for review Correct

**Domain:** Develop a security and compliance plan

A team is currently building and deploying an application using Azure DevOps services. You have to use the right security tool during the following phase of the development lifecycle.

- After a pull request
- During the continuous integration phase
- During the continuous delivery phase

Which of the following would you use for the continuous delivery phase?

- A. Penetration Testing right
- B. Static Code Analysis
- C. Threat Modeling
- D. Load Testing

###### Explanation:

**Answer – A**

During the deployment phase, we can use Penetration testing tools. The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_8.png)  
**Option A is CORRECT** since Penetration testing should be used during the deployment phase.

**Option B is incorrect** since Static Code Analysis should be used during the development phase.

**Option C is incorrect** since the Threat Modeling tool should be used during the design phase.  
  
**Option D is incorrect** because load testing is used to check the performance and not the security of the application.

For more information on security during the DevOps lifecycle, please visit the below URL-

- [https://docs.microsoft.com/en-us/shows/azure-enablement/devsecops-bringing-security-into-your-devops-practice-on-azure](https://docs.microsoft.com/en-us/shows/azure-enablement/devsecops-bringing-security-into-your-devops-practice-on-azure)

Question 9 Correct

**Domain:** Design and implement processes and communications

A team is currently building and deploying an application using Azure DevOps services. The development team needs to have an efficient way to communicate with each other. The tool should have the following capabilities.

- Provide the ability to have different communication channels for each team.
- Have the ability to integrate with Azure DevOps.
- Should be available for a variety of platforms such as Windows 10, Mac OS, iOS, and Android.

Which of the following would you use for this purpose?

- A. Microsoft Project
- B. Slack right
- C. Jenkins
- D. Bamboo

###### Explanation:

**Answer – B**

Slack is the perfect communication tool for this requirement. The following snippet from azure marketplace provides an overview of slack.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_9.png)

**Option A is incorrect** since Microsoft Project is a project management tool.

**Option B is CORRECT** since Slack is a communication tool and it has good support for Azure DevOps integrations also it satisfies all other requirements mentioned in the question.

**Option C is incorrect** since Jenkins is a continuous integration tool.

**Option D is incorrect** since Bamboo is a continuous integration tool.

For more information on the tool, please visit the below URL-

- [https://marketplace.visualstudio.com/items?itemName=ms-vsts.vss-services-slack](https://marketplace.visualstudio.com/items?itemName=ms-vsts.vss-services-slack)
- [https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/slack?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/slack?view=azure-devops)

Question 10 Correct

**Domain:** Design and implement processes and communications

A team needs to track project metrics in the dashboards available in Azure DevOps.  
You need to recommend the right chart widgets to use for each of the following requirements.

- Ability to provide the elapsed time from the creation of work items to their completion.
- Ability to provide the elapsed time to complete work items once they are marked as active.
- Ability to provide a view of the work remaining.

Which of the following chart widget would you use for the following requirement?  
**“Ability to provide the elapsed time from the creation of work items to their completion.”**

- A. Burndown
- B. Cycle Time
- C. Lead Time right
- D. Velocity

###### Explanation:

**Answer – C**

You can use the Lead time chart for this. The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_10.png)

**Option A is incorrect** because the Burndown widget displays a trend of remaining work across multiple teams and multiple sprints.

**Option B is incorrect** because the Cycle Time widget helps to analyze the time it takes for a team to complete work items once they are marked as active.

**Option C is CORRECT** because Lead Time measures the total time elapsed from the creation of work items to their completion.

**Option D is incorrect** because the Velocity widget helps to learn how much work a team can complete during a sprint.

For more information on the widgets, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/report/dashboards/analytics-widgets?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/report/dashboards/analytics-widgets?view=azure-devops)

Question 11 Correct

**Domain:** Design and implement processes and communications

A team needs to track project metrics in the dashboards available in Azure DevOps.

You need to recommend the right chart widgets to use for each of the following requirements.

- Ability to provide the elapsed time from the creation of work items to their completion
- Ability to provide the elapsed time to complete work items once they are marked as active
- Ability to provide the view on the work remaining

Which of the following chart widget would you use for the following requirement?

**“Ability to provide the elapsed time to complete work items once they are marked as active.”**

- A. Burndown
- B. Cycle Time right
- C. Lead Time
- D. Velocity

###### Explanation:

Answer – B

You can use the Cycle time chart for this. The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_11.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on the widgets, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/report/dashboards/analytics-widgets?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/report/dashboards/analytics-widgets?view=azure-devops)

Question 12 Marked for review Incorrect

**Domain:** Design and implement processes and communications

A team needs to track project metrics in the dashboards available in Azure DevOps.

You need to recommend the right chart widgets to use for each of the following requirements.

- Ability to provide the elapsed time from the creation of work items to their completion
- Ability to provide the elapsed time to complete work items once they are marked as active
- Ability to provide the view on the work remaining

Which of the following chart widget would you use for the following requirement?

**“Ability to provide the view on the work remaining.”**

- A. Burndown right
- B. Cycle Time
- C. Lead Time
- D. Velocity wrong

###### Explanation:

Answer - A

You can use the Burndown chart for this. The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_12.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on the widgets, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/report/dashboards/analytics-widgets?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/report/dashboards/analytics-widgets?view=azure-devops)

Question 13 Correct

**Domain:** Design and implement build and release pipelines

A company has created a new project in Azure DevOps for a web application. The company currently uses ServiceNow for change and release management. The company wants to ensure that a change request is processed before any changes are released to production. Which of the following are the two ways that ServiceNow can be integrated into the Azure DevOps Release pipeline?

- A. Create a deployment control that invokes the ServiceNow SOAP API.
- B. Configure deployment conditions using the 'Azure Invoke REST API' gate.right
- C. Configuring deployment conditions using the ServiceNow DevOps extension for 'Azure DevOps' gate.right
- D. Configure deployment conditions using the Invoke 'Azure Function' gate.

###### Explanation:

**Answer – B and C**

You can configure change control in Azure pipelines in two ways:

1. Use the Azure Invoke REST API.
2. Use the ServiceNow DevOps extension for Azure DevOps.

The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_13.png)

**Option A is incorrect** because we do not have support for SOAP web service request in release pipeline deployment conditions gate

**Option B is CORRECT** because in the release pipeline deployment conditions gate we have "Invoke REST API" gate to query data using REST API, this is also suggested in Servicenow documentation.

**Option C is CORRECT** because after installing the ServiceNow DevOps extension from the marketplace we get "ServiceNow change management" gate in release pipeline deployment conditions.

**Option D is incorrect** because "Invoke Azure Function" gate in release pipeline deployment conditions is for querying the azure function.

For more information on using ServiceNow with Azure DevOps, please visit the below URLs-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/servicenow?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/servicenow?view=azure-devops)
- [https://docs.servicenow.com/bundle/sandiego-devops/page/product/enterprise-dev-ops/concept/config-azure-pipeline-dev-ops.html](https://docs.servicenow.com/bundle/sandiego-devops/page/product/enterprise-dev-ops/concept/config-azure-pipeline-dev-ops.html)

Question 14 Marked for review Incorrect

**Domain:** Design and implement a source control strategy View Case Study  

Fabrikam Inc. needs to configure permissions in their Azure DevOps Git repositories to ensure that developers, team leaders, and project managers have the appropriate level of access. The solution should adhere to the principle of least privilege.

Which of the following configurations should Fabrikam implement for each requirement?

Note: To achieve the above requirement you need to match the option by dragging the correct options from the Users Responsibilities and dropping them in the Roles \[correct answer area\].

- **Your Answers**
- Triage
- Developer - should be able to create and work on feature branches
- Maintain
- Project Manager - should have admin privileges without the ability to perform sensitive actions like deleting the repository
- Write
- Team Leader - should be able to manage issues, discussions, and pull requests
- **Correct Answers**
- Triage
- Team Leader - should be able to manage issues, discussions, and pull requests
- Maintain
- Project Manager - should have admin privileges without the ability to perform sensitive actions like deleting the repository
- Write
- Developer - should be able to create and work on feature branches

###### Explanation:

**Correct Answer: 1-C, 2-A, 3-B**

- **Triage**

**Team Leader - should be able to manage issues, discussions, and pull requests**

- **Maintain**

**Project Manager - should have admin privileges without the ability to perform sensitive actions like deleting the repository**

- **Write**

**Developer - should be able to create and work on feature branches**

**Triage Role:**

Assign the Triage role to the Team Leader. This role is suitable for managing issues, discussions, and pull requests without write access. It allows the Team Leader to oversee project progress effectively and facilitate collaboration among team members, ensuring tasks are addressed and discussions are managed efficiently.

**Maintain Role:**

Assign the Maintain role to the Project Manager. This role grants administrative privileges necessary for managing the repository without the ability to perform sensitive or destructive actions like deleting the repository. It allows the Project Manager to oversee project progress, manage team assignments, and ensure project milestones are met, maintaining project integrity and security.

**Write Role:**

Assigning the Write role to Developers grants them permission to create and collaborate on feature branches, empowering them to actively contribute to the codebase. This role enables developers to push changes, initiate branches, and engage in effective collaboration with team members, thereby maintaining seamless development workflows while upholding the principle of least privilege.

**References:**

- [https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#repository-roles-for-organizations](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#repository-roles-for-organizations)
- [https://learn.microsoft.com/en-us/training/modules/manage-git-repositories/12-configure-source-control-repository-permissions-use-github?ns-enrollment-type=learningpath&ns-enrollment-id=learn.wwl.az-400-work-git-for-enterprise-devops](https://learn.microsoft.com/en-us/training/modules/manage-git-repositories/12-configure-source-control-repository-permissions-use-github?ns-enrollment-type=learningpath&ns-enrollment-id=learn.wwl.az-400-work-git-for-enterprise-devops)

Question 15 Correct

**Domain:** Develop a security and compliance plan

A team needs to deploy resources using Azure Resource Manager templates. You have to ensure the security for the users performing the deployment. They cannot view the connection strings required by the application being deployed via the template. Which of the following would you use for this requirement?

- A. A parameter file
- B. A Storage account
- C. Azure Key vault right
- D. Web.config file

###### Explanation:

Answer – C

The ideal service to use for this purpose is the Azure Key Vault service. The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_15.png)

All other options are incorrect since the ideal service to use for this requirement is the Azure Key Vault service.

For more information on using the Azure Key Vault service to protect application secrets, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/architecture/multitenant-identity/key-vault](https://docs.microsoft.com/en-us/azure/architecture/multitenant-identity/key-vault)

Question 16 Correct

**Domain:** Design and implement a source control strategy

A team is currently working on a repository in Azure Repos for managing all of the source code. There are a high number of feature requests. That makes it difficult to follow the history of the changes to the master branch. You need to enforce a merge strategy that would

- Allows consolidation of all commit histories
- Merge the changes into a single commit

You decide to implement the squash merge strategy.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

**Answer – A**

Yes, this would fulfill the desired requirement. The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_16.png)

For more information on squash merge, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/merging-with-squash?view=azure-devops)

Question 17 Marked for review Correct

**Domain:** Design and implement a source control strategy

A team is currently working on a repository in Azure Repos for managing all of the source code. There are a high number of feature requests. That makes it difficult to follow the history of changes to the master branch. You need to enforce a strategy that would

- Allows consolidation of all commit histories
- Merge the changes into a single commit

You decide to implement a pull request template.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

The pull request template is a file containing [markdown](https://docs.microsoft.com/en-us/azure/devops/project/wiki/markdown-guidance?view=azure-devops) text that is added to your pull request description when the pull request is created.

For more information on pull request templates, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/pull-request-templates?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/pull-request-templates?view=azure-devops)

Question 18 Correct

**Domain:** Design and implement a source control strategy

A team is currently working on a repository in Azure repo’s for managing all of the source code. There are a high number of feature requests. So, that makes it difficult to follow the history of the changes to the master branch. You need to enforce a strategy that would

- Allows consolidation of all commit histories
- Merge the changes into a single commit

You decide to implement a git fetch request.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

The git fetch request is used to download objects from another repository.

For more information on git fetch, please visit the below URL-

- [https://git-scm.com/docs/git-fetch](https://git-scm.com/docs/git-fetch)

Question 19 Correct

**Domain:** Design and implement build and release pipelines

You are configuring an Azure DevOps pipeline and need to automatically infer test results. Which of the following languages and test runners are supported by Azure DevOps for automatic inference of test results? (Select two)

- A. JavaScript - Mocha, Jest, and Jasmine right
- B. Ruby - RSpec
- C. Java - JUnit, and TestNG
- D. Python - PyTest
- E. Python - Unittest right

###### Explanation:

**Correct Answer: A and E**

- **Option A is CORRECT** because Azure DevOps supports automatic inference of test results for the JavaScript test runners Mocha, Jest, and Jasmine. These test runners are recognized by Azure DevOps, which can parse their error logs and infer test results automatically.
- **Option E is CORRECT** because Azure DevOps supports automatic inference of test results for Python's Unittest framework. This allows Azure DevOps to parse error logs from Unittest and infer the test results without additional configuration.
- **Option B is INCORRECT** because Azure DevOps does not support automatic inference of test results for Ruby's RSpec test runner. RSpec is not listed among the test runners that Azure DevOps can automatically infer test results from.
- **Option C is INCORRECT** because Azure DevOps does not automatically infer test results for Java test runners like JUnit and TestNG. These test runners are not included in the list of supported test runners for automatic inference.
- **Option D is INCORRECT** because PyTest for Python is not supported by Azure DevOps for automatic inference of test results. Only Python's Unittest is supported.

**Reference:**

- [Review test results - Azure Pipelines | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/pipelines/test/review-continuous-test-results-after-build?view=azure-devops#surface-test-results-in-the-tests-tab)

Question 20 Correct

**Domain:** Implement an instrumentation strategy

You need to query the log tables using Kusto Query Language.

What are two Azure tools that can help you write a KQL query?

- A. Azure Function App
- B. Azure Data Explorer right
- C. Application Insights
- D. Azure SQL
- E. Log Analytics right

###### Explanation:

**Correct Answers: B and E**

Microsoft Azure Monitor stores two types of data: logs and metrics. This data helps users monitor, tune, and troubleshoot their applications and services. Azure Monitor collects data from applications, operating systems, Azure resources, subscriptions, tenants, and custom sources.

Logs data are the records that contain predominantly text information but can include numeric data as well. Typically, logs store event information from a variety of sources. Azure Monitor creates a table for each log source to store its data and uses Log Analytics workspace as a data storage.

There are two tools that Azure provides to create Kusto Query Language (KQL) queries: Azure Data Explorer and Log Analytics. Both tools include the data browser and query editor. Users can use IntelliSense for writing a query.

Here is a screenshot for Azure Data Explorer.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/az4-1.1.jpg)

And a screenshot for Log Analytics.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/az4-1.2.jpg)

- **Options A, C, and D are incorrect** because these tools do not provide a workspace for creating KQL queries.

For more information about Kusto Query Language tools, please visit the below URLs:

- [https://docs.microsoft.com/en-us/azure/azure-monitor/logs/data-platform-logs#log-queries](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/data-platform-logs#log-queries)
- [https://docs.microsoft.com/en-us/azure/data-explorer/data-explorer-overview](https://docs.microsoft.com/en-us/azure/data-explorer/data-explorer-overview)
- [https://docs.microsoft.com/en-us/azure/azure-monitor/logs/log-analytics-overview#log-analytics-interface](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/log-analytics-overview#log-analytics-interface)

Question 21 Correct

**Domain:** Design and implement a source control strategy View Case Study  

You need to comply with the requirement for the project “whizlabD”. Which of the following would you set for the folder /\*?

- A. A branch filter to exclude -data/\*
- B. A branch filter to include -data/\*
- C. A path filter to include -data/\*
- D. path filter to exclude -data/\* right

###### Explanation:

**Answer – D**

The branch name has not been mentioned in the question for ProjectD. So the branch name will be default i.e. master.  
In the yaml file, we will specify "- /\*" folder under "exclude:" element under "paths:" element under default branch "master: " of the project "ProjectD"

When you specify paths, you must explicitly specify branches to trigger on. You can't trigger a pipeline with only a path filter; you must also have a branch filter, and the changed files that match the path filter must be from a branch that matches the branch filter.

Below snippet shows the syntax for excluding content inside folder:

![](https://s3.amazonaws.com/media.whizlabs.com/learn/az400-pathfilter.PNG)  
**Option A is incorrect** because a branch filter is applied when we have multiple branches under the same project.  
**Option B is incorrect** because a branch filter is applied when we have multiple branches under the same project.  
**Option C is incorrect** because the requirement is to exclude the content inside the data folder and not to include them.  
**Option D is CORRECT** because this will exclude the content inside the data folder, the syntax is as per Microsoft documentation.

For more information on path filters, refer to the below URL:

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml#ci-triggers](https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml#ci-triggers)

Question 22 Correct

**Domain:** Design and implement build and release pipelines View Case Study  

You need to implement the requirement for the project “whizlabF”. Which of the following steps would you apply for this requirement? Choose three answers from the options given below.

- A. Use the release pipeline editor.right
- B. Use the triggers tab.
- C. Make sure to enable gates.right
- D. Ensure to add a manual intervention task.
- E. Ensure to Add Query Work items.right

###### Explanation:

Answer – A, C and E

You can add gates that can be used to validate whether there is no active bug against the application. The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_22.1.png)

You can put up queries to search for values of interest, which can be used by then. The below snapshots from the Microsoft documentation showcases how this can be achieved.

First, go to the release pipeline editor.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_22.2.png)

Then Query for Work Items

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_22.3.png)

Then define the condition for the work items

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_22.4.png)

Since this is clearly mentioned in the documentation, all other options are incorrect.

For more information on gates, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/gates?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/gates?view=azure-devops)

Question 23 Correct

**Domain:** Implement an instrumentation strategy

Your team is setting up a DevOps environment in Azure. As part of the setup, several development environments are going to be spun up in Azure. Several Azure Resource Manager templates are going to be used to create the various development environments. You have to monitor all of the control-plane events.

You decide to use Azure Storage Analytics for monitoring all of the control-plane activities.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

Azure Storage Analytics is used to provide insight into trace requests, usage trends, and issues with your storage account.

For this requirement, you have to use the Activity logs service.

For more information on logs and audits, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/security/fundamentals/log-audit](https://docs.microsoft.com/en-us/azure/security/fundamentals/log-audit)

Question 24 Correct

**Domain:** Implement an instrumentation strategy

Your team is setting up a DevOps environment in Azure. As part of the setup, several development environments are going to be spun up in Azure. Several Azure Resource Manager templates are going to be used to create the various development environments. You have to monitor all of the control-plane events.

You decide to use Azure Activity logs for monitoring all of the control-plane activities.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

Answer – A

Yes, this is the right approach.

The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_24.png)

For more information on logs and audits, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/security/fundamentals/log-audit](https://docs.microsoft.com/en-us/azure/security/fundamentals/log-audit)

Question 25 Marked for review Correct

**Domain:** Implement an instrumentation strategy

Your team is setting up a DevOps environment on Azure. As part of the setup, several development environments are going to be spun up in Azure. Several Azure Resource Manager templates are going to be used to create the various development environments. You have to monitor all of the control-plane events.

You decide to use Network Security Group Flow logs for monitoring all of the control-plane activities.

Would this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

Answer – B

This is used to capture ingress and egress IP traffic that flows via Network Security groups.

For this requirement, you have to use the Activity logs service.

For more information on logs and audits, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/security/fundamentals/log-audit](https://docs.microsoft.com/en-us/azure/security/fundamentals/log-audit)

Question 26 Incorrect

**Domain:** Design and implement build and release pipelines

You need to set up a pipeline in Azure DevOps to ensure that code coverage metrics are evaluated for pull requests. Which configuration file should you add to your repository to change the default settings for code coverage checks?

- A. azure-pipelines.yml wrong
- B. azurepipelines-coverage.yml right
- C. azure-pipelines-coverage.yml
- D. azurepipelines-config.yml

###### Explanation:

**Correct Answer: B**

- **Option B is CORRECT** because ‘azurepipelines-coverage.yml’ is the correct file for configuring code coverage settings for pull requests in Azure DevOps. This file allows you to set parameters such as coverage status checks, diff coverage targets, and whether to post comments with coverage details.
- **Option A is INCORRECT** because ‘azure-pipelines.yml’ is the primary configuration file for defining the pipeline itself. This file is used to specify the pipeline steps, tasks, and triggers, but it does not specifically configure code coverage settings for pull requests.
- **Option C is INCORRECT** because ‘azure-pipelines-coverage.yml’ is not the correct name for the configuration file used to set code coverage settings in Azure DevOps.
- **Option D is INCORRECT** because ‘azurepipelines-config.yml’ is not a recognized configuration file for setting code coverage metrics or any other specific pipeline settings in Azure DevOps.

**Reference:**

- [https://learn.microsoft.com/en-us/azure/devops/pipelines/test/codecoverage-for-pullrequests?view=azure-devops#configuring-coverage-settings](https://learn.microsoft.com/en-us/azure/devops/pipelines/test/codecoverage-for-pullrequests?view=azure-devops#configuring-coverage-settings)

Question 27 Correct

**Domain:** Implement an instrumentation strategy

Which of the following in Application Insights would you use for the following requirement?

**“Where do users churn the most from the application”**

- A. Funnels
- B. Cohorts
- C. Impact
- D. Retention
- E. User Flows right

###### Explanation:

Answer – E

You can use User Flows for this requirement

The Microsoft documentation mentions the following

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_27.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect

For more information on Application Insights – User Flows, please refer to the following link

- [https://docs.microsoft.com/en-us/azure/azure-monitor/app/usage-flows](https://docs.microsoft.com/en-us/azure/azure-monitor/app/usage-flows)

Question 28 Correct

**Domain:** Implement an instrumentation strategy

Which of the following Application Insights would you use for the following requirement?

**“Are page load times affecting a user’s decision in continuing to use the application.”**

- A. Funnels
- B. Cohorts
- C. Impact right
- D. Retention
- E. User Flows

###### Explanation:

Answer – C

You can use the Impact feature for this requirement.

The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_28.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on Application Insights – Impact, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/azure-monitor/app/usage-impact](https://docs.microsoft.com/en-us/azure/azure-monitor/app/usage-impact)

Question 29 Correct

**Domain:** Design and implement build and release pipelines

You have to deploy a set of Azure Virtual Machines that will sit behind an Azure Load Balancer. The Virtual Machines will have a web site hosted on them. Users will be accessing the web site via the URL [https://whizlabs.com](https://whizlabs.com/).

You have to implement probes based on HTTPS. You have to ensure that costs are reduced in the implementation process.

Which of the following would you choose as the underlying SKU type for the Load Balancer?

- A. Basic
- B. Standard right
- C. Premium
- D. Isolated

###### Explanation:

Answer – B

The Azure Load balancer has two SKU types: Basic and Standard.

The Standard SKU supports the HTTPS probe type.

The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_29.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on probes for the Azure Load Balancer – Impact, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/load-balancer/load-balancer-custom-probe-overview](https://docs.microsoft.com/en-us/azure/load-balancer/load-balancer-custom-probe-overview)

Question 30 Correct

**Domain:** Implement an instrumentation strategy

You are designing the log aggregation query strategy using Azure Monitor.

What two types of data does Azure Monitor store?

- A. Insights
- B. Metrics right
- C. Forecasts
- D. Logs right
- E. Scripts

###### Explanation:

**Correct Answers: B and D**

Microsoft Azure Monitor stores two types of data: **logs** and **metrics**. This data helps users to monitor, tune and troubleshoot their applications and services. Azure Monitor collects data from applications, operating systems, Azure resources, subscriptions, tenants, and custom sources.

**Logs** data are the records that contain predominantly text information but can include numeric data as well. Typically logs store event information from a variety of sources. Azure Monitor creates a table for each log source to store its data and uses Log Analytics workspace as a data storage. You can use Azure Monitor tools or Azure Data Explorer to query logs data with the help of Kusto Query Language (KQL).

**Metrics** data is numeric information that you can collect from services such as Application Insights. It includes metric telemetry data like request rates, response times, performance counters, etc. This type of data is collected in the Metric part of the Azure Monitor. The structure of the Metric data differs from the Log Analytics data. Metric data is stored in time-series databases. These databases are optimized for analyzing time-stamped data. To work with Metric data, you can use Azure Metrics Explorer or other tools to analyze telemetry data details, like Application maps, Profiler, Dashboards, etc.

All other options are incorrect.

For more information about the Azure Monitor data types, please visit the below URL:

- [https://docs.microsoft.com/en-us/azure/azure-monitor/overview](https://docs.microsoft.com/en-us/azure/azure-monitor/overview)
- [https://docs.microsoft.com/en-us/learn/modules/analyze-infrastructure-with-azure-monitor-logs/2-features-azure-monitor-log](https://docs.microsoft.com/en-us/learn/modules/analyze-infrastructure-with-azure-monitor-logs/2-features-azure-monitor-log)

Question 31 Correct

**Domain:** Develop a security and compliance plan

Your team is now developing applications. They are built around docker containers. You are planning to push the images and store them in the Azure container registry. Several application environments in Azure would then pull these images and run them as containers.

You have to ensure service principals are used to access the Azure container registry. You have to provide the credentials for the service principal and ensure that they are stored in an existing Azure key vault instance.

You have to complete the below Azure CLI command to implement this requirement.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_32-33.png)

Which of the following would go into Slot 1?

- A. az keyvault set
- B. az keyvault secret set right
- C. az ad sp create-for-rbac
- D. az ad create

###### Explanation:

Answer – B

Here we have to set the value of the secret in the key vault.

An example of this is given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_31.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on an example on Azure container registry tasks, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-quick-task](https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-quick-task)

Question 32 Correct

**Domain:** Develop a security and compliance plan

Your team is currently developing applications. They are built around docker containers. You are planning to push the images and store them in the Azure container registry. Several application environments in Azure would then pull these images and run them as containers.

You have to ensure service principals are used to access the Azure container registry. You have to provide the credentials for the service principal and ensure that they are stored in an existing Azure key vault instance.

You have to complete the below Azure CLI command to implement this requirement.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_32-33_47_59.png)

Which of the following would go into Slot 2?

- A. az keyvault set
- B. az keyvault secret set
- C. az ad sp create-for-rbac right
- D. az ad create

###### Explanation:

**Answer – C**

In Slot 2 we have to go ahead and create the service principal in Azure AD for which "az ad sp create-for-rbac" command is used.

An example of this is given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_32.png)

**Option A is incorrect** because this is not a complete command, the complete command text is "az keyvault set-policy" which is used for updating the security policy settings for key-vault.

**Option B is incorrect** because this command is used for creating a secret (if one doesn't exist) or updating a secret in a KeyVault.

**Option C is CORRECT** because this command is used for creating service principal in Azure AD which is the correct fit for Slot 2.

**Option D is incorrect** because this is not a valid command, it's also not available in Microsoft documentation.

For more information on an example of Azure container registry tasks and azure key vault secret set command, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-quick-task](https://docs.microsoft.com/en-us/azure/container-registry/container-registry-tutorial-quick-task)
- [https://docs.microsoft.com/en-us/cli/azure/keyvault/secret?view=azure-cli-latest#az-keyvault-secret-set](https://docs.microsoft.com/en-us/cli/azure/keyvault/secret?view=azure-cli-latest#az-keyvault-secret-set)

Question 33 Correct

**Domain:** Design and implement a source control strategy

Your team currently makes use of Azure Pipelines. You have to configure Azure Pipelines to pick up code from various GitHub repositories. You have to create a continuous integration trigger that would cause the pipeline to run based on the following event.

- Whenever a change is pushed to any of the master or release branches
- Ensure that the pipeline does not run when a change is made to a specific archive release branch.

You have to complete the below YAML configuration for this requirement.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_33-34.png)

Which of the following would go into Slot 1?

- A. github
- B. pipeline
- C. include right
- D. exclude

###### Explanation:

Answer – C

Since we have to include the master and release branches, we will use the included statement in the YAML configuration.

An example of this is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_33.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on integrating Github with Azure Pipelines, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml)

Question 34 Correct

**Domain:** Design and implement a source control strategy

Your team currently uses Azure Pipelines. You have to configure Azure Pipelines to pick up code from various GitHub repositories. So, you need to create a continuous integration trigger that would cause the pipeline to run based on the following event.

- Whenever a change is pushed to any of the master or release branches
- Ensure that the pipeline does not run when a change is made to a specific archive release branch.

You have to complete the below YAML configuration for this requirement.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_33-34_54_22.png)

Which of the following would go into Slot 2?

- A. github
- B. pipeline
- C. include
- D. exclude right

###### Explanation:

Answer – D

Since we have to exclude the archive release branch, we will use the excluded statement in the YAML configuration.

An example of this is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_34.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on integrating Github with Azure Pipelines, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml)

Question 35 Correct

**Domain:** Design and implement processes and communications

Your team currently has code hosted in a Github repository. You have to connect your Azure Board Project with a GitHub.com repository.

Which of the following groups you should be a member of in your Azure DevOps project to connect to GitHub from Azure Boards?  
Choose two answers from the options given below. Each answer presents part of the solution.

- A. Reader Group
- B. Project Collection Administrators Group right
- C. Project’s Contributors Group right
- D. GitHub Group

###### Explanation:

**Answer – B and C**

For connecting your Azure board with a GitHub.com repository below is one of the prerequisites:

"You must be a member of the [**Project Collection Administrators** group](https://docs.microsoft.com/en-us/azure/devops/organizations/security/change-organization-collection-level-permissions?view=azure-devops)  and the project's  [Contributors group](https://docs.microsoft.com/en-us/azure/devops/organizations/security/add-users-team-project?view=azure-devops) "

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/az400-groups.PNG)

**Option A is incorrect** because with the reader's group users can view project information, the code base, work items, and other artifacts but not modify them. The user can not connect azure board with GitHub repository.

**Option B is CORRECT** because one of the group permission required for connecting azure board with GitHub repository is "Project Collection Administrator".

**Option C is CORRECT** because one of the group permission required for connecting azure board with GitHub repository is "Contributor".

**Option D is incorrect** because GitHub group-related permissions are not required for this.

For more information on connecting to GitHub from Azure Boards, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/devops/boards/github/connect-to-github?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/boards/github/connect-to-github?view=azure-devops)

Question 36 Correct

**Domain:** Design and implement processes and communications

Your team currently has code hosted in a Github repository. You have to connect an Azure Boards project with a GitHub.com repository.

Which of the following permissions must be given to a user for the GitHub repository to connect to GitHub from Azure Boards? Choose two answers from the options given below. Each answer presents a complete solution.

- A. Administrator right
- B. Owner right
- C. Reader
- D. Default

###### Explanation:

Answer – A and B

You must be either the administrator or owner of the GitHub repository.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_36.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on connecting to GitHub from Azure Boards, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/devops/boards/github/connect-to-github?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/boards/github/connect-to-github?view=azure-devops)

Question 37 Correct

**Domain:** Design and implement build and release pipelines

Your team is working on the development of an application that will be deployed on Azure. They are planning to use Azure Pipelines for continuous integration and release of the application. They need to enable continuous monitoring of the release pipelines.  
Which of the following option can be used in the Release pipeline to achieve this requirement?

- A. Use Query Azure Monitor alerts deployment gate right
- B. Check Azure Policy Compliance deployment gate
- C. Release Annotations
- D. Release monitoring

###### Explanation:

**Answer – A**

You can use Query Azure Monitor alerts deployment gate to achieve this requirement. When you add deployment gates to your release pipeline, an alert that exceeds the thresholds you set prevents unwanted release promotion. Once you resolve the alert, the deployment can proceed automatically.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/monitoring.PNG)

**Option A is CORRECT** because the deployment gate can be used to hold the release till the alerts raised by the 'Query Azure Monitor alerts' gate are resolved.

**Option B is incorrect** because the 'Check Azure Policy Compliance' gate is used for security and compliance assessment for azure policies.

**Option C is incorrect** because Release annotations allow us to add markers in Application Insights to note when we completed a release. After implementing Release annotations we get more information to troubleshoot performance changes.

**Option D is incorrect** because we trying to achieve release monitoring using options available in the release pipeline.

For more information on continuous monitoring in your release pipeline, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/azure-monitor/app/continuous-monitoring](https://docs.microsoft.com/en-us/azure/azure-monitor/app/continuous-monitoring)

Question 38 Correct

**Domain:** Design and implement build and release pipelines

Your company wants to use Azure Artifacts for hosting a private PowerShell repository. This would allow multiple teams to download and upload PowerShell modules. Which of the following steps would you implement for this requirement?

- **Your Answer**
- C. Create a new feed within Azure Artifacts
- B. Create a Personal Access Token (PAT) to authenticate other services with Azure DevOps
- F. Connect to feed as a PowerShell repository and with Azure Pipelines
- E. Create, package, and publish PowerShell modules with Azure Artifacts Feed
- **Correct Answer**
- B. Create a Personal Access Token (PAT) to authenticate other services with Azure DevOps
- C. Create a new feed within Azure Artifacts
- E. Create, package, and publish PowerShell modules with Azure Artifacts Feed
- F. Connect to feed as a PowerShell repository and with Azure Pipelines

###### Explanation:

**Correct Answer: B, C, E and F**

- **Create a Personal Access Token (PAT) to authenticate other services with Azure DevOps.**
- **Create a new feed within Azure Artifacts.**
- **Create, package, and publish PowerShell modules with Azure Artifacts Feed.**
- **Connect to feed as a PowerShell repository and with Azure Pipelines**

This is also given as an example in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/PT-1-Q38.png)

Since this is clearly mentioned in the Microsoft documentation,

all other options are incorrect.

**Reference:**

- [Use Azure Artifacts feeds as a private PowerShell repository - Azure Artifacts | Microsoft Docs](https://docs.microsoft.com/en-us/azure/devops/artifacts/tutorials/private-powershell-library?view=azure-devops)

Question 39 Correct

**Domain:** Design and implement build and release pipelines

A team is currently using Azure Pipelines for their application deployments. They now want to implement database updates to an Azure SQL database after every successful build. Which of the following steps the team can apply for this requirement?

###### Explanation:

**Answer – B and C**

You can publish schema-related changes using a DACPAC. You can then use the Azure SQL Database deployment task in Azure Pipelines.

This is also mentioned in the Microsoft documentation-

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_39.1.png)

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_39.2.png)

**Option A is incorrect** because ARM templates can be used for the creation of Azure SQL database resources but not for database updates.

**Option B is the CORRECT** step because for database change deployment you can create DACPA. DACPACs can be used to package and deploy schema changes and data.

**Option C is the CORRECT** step because, for the deployment of the DACPAC file, you need to use this task.

**Option D is incorrect** because this task can not be used for database updates.

For more information on publishing changes to an Azure SQL database, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/targets/azure-sqldb](https://docs.microsoft.com/en-us/azure/devops/pipelines/targets/azure-sqldb)

Question 40 Correct

**Domain:** Design and implement build and release pipelines

When creating pipelines in Azure Pipelines for GitHub repositories, what is the default name given to the repository in which the YAML file resides?

- A. self right
- B. default
- C. main
- D. primary

###### Explanation:

**Correct Answer: A**

- **Option A is CORRECT** because when creating pipelines in Azure Pipelines for GitHub repositories, the default name given to the repository in which the YAML file resides is "self." This means that by default, the pipeline configuration YAML file in the repository will refer to the same repository for building and deployment processes.
- **Option B is INCORRECT** because the term "default" is not used as the default name for the repository in Azure Pipelines. It is not relevant to the default naming convention in Azure Pipelines for repositories.
- **Option C is INCORRECT** because the term "main" is not used as the default name for the repository in Azure Pipelines. It is not relevant to the default naming convention in Azure Pipelines for repositories.
- **Option D is INCORRECT** because the term "primary" is not used as the default name for the repository in Azure Pipelines. It is not relevant to the default naming convention in Azure Pipelines for repositories.

**Reference:**

- [https://learn.microsoft.com/en-us/training/modules/implement-pipeline-strategy/4-integrate-github-repos-azure-pipelines?ns-enrollment-type=learningpath&ns-enrollment-id=learn.wwl.az-400-implement-ci-azure-pipelines-github-actions](https://learn.microsoft.com/en-us/training/modules/implement-pipeline-strategy/4-integrate-github-repos-azure-pipelines?ns-enrollment-type=learningpath&ns-enrollment-id=learn.wwl.az-400-implement-ci-azure-pipelines-github-actions)

Question 41 Correct

**Domain:** Design and implement build and release pipelines

You have recently joined the DevOps team at Contoso, a software development company. As part of your responsibilities, you are tasked with setting up Azure Pipelines to build and deploy code from GitHub repositories. Which authentication type(s) can you use to grant Azure Pipelines access to your GitHub repositories? (Select three)

- A. SSH Key
- B. API Key
- C. GitHub App right
- D. OAuth right
- E. Personal Access Token (PAT) right

###### Explanation:

**Correct Answers: C, D and E**

- **Option C is CORRECT** because GitHub App authentication is one of the supported methods for granting Azure Pipelines access to GitHub repositories. GitHub Apps can be installed in GitHub organizations or user accounts, and Azure Pipelines can use the GitHub App's identity to authenticate and interact with repositories.
- **Option D is CORRECT** because OAuth authentication is supported for granting Azure Pipelines access to GitHub repositories. OAuth allows Azure Pipelines to act on behalf of users or organizations with the necessary permissions when interacting with GitHub repositories.
- **Option E is CORRECT** because Personal Access Tokens (PATs) are supported for granting Azure Pipelines access to GitHub repositories. PATs provide a way to authenticate as a user or an application and can be used to access GitHub resources securely.
- **Option A is INCORRECT** because Azure Pipelines does not support SSH Key authentication for accessing GitHub repositories. SSH keys are typically used for authentication between Git clients and Git servers, but Azure Pipelines integrates with GitHub using other authentication methods.
- **Option B is INCORRECT** because Azure Pipelines does not use API keys for accessing GitHub repositories. API keys are used for accessing APIs directly, but Azure Pipelines uses other authentication methods when interacting with GitHub repositories.

**Reference:**

- [https://learn.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml#access-to-github-repositories](https://learn.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml#access-to-github-repositories)

Question 42 Incorrect

**Domain:** Design and implement build and release pipelines

Your company is currently using Azure Pipelines for application deployment. They want to use Azure Pipelines in order to deploy Azure Resource Manager Templates. Which of the following are two ways to deploy templates with Azure Pipelines? Choose two answers from the options given below.

- A. Create a Resource Group deployment task wrong
- B. Add a task that runs an Azure PowerShell script.right
- C. Add tasks to copy and deploy tasks.right
- D. Add an Azure Blueprint task.

###### Explanation:

Answer – B and C

The two ways given in the Microsoft documentation for the deployment of Azure Resource Manager Templates as part of Azure Pipelines are

1. Add a task that runs an Azure PowerShell script.
2. Add tasks to copy and deploy tasks.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_42.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on adding templates to Azure Pipelines, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/add-template-to-azure-pipelines](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/add-template-to-azure-pipelines)

Question 43 Incorrect

**Domain:** Implement an instrumentation strategy

You need to query the log data in Azure Monitor.

Please select the two types of queries that you can create?

- A. Logic
- B. Table-based right
- C. Workspace wrong
- D. Security
- E. Search right

###### Explanation:

**Correct Answers: B and E**

Microsoft Azure Monitor data helps users to monitor, tune and troubleshoot their applications and services. Azure Monitor collects data from applications, operating systems, Azure resources, subscriptions, tenants, and custom sources.

In Azure Monitor, you use Kusto Query Language (KQL) to query the logs and retrieve the log’s data.

There are two types of queries that you can create: **Table-based** and **Search**.

The **table-based** query starts with the table name (Number 1) and, using the pipes (|), chains the filtering conditions (lines 2 and 3, Number 2). Then summarizes and sorts the query result and renders the chart (lines 4-6, Number 3).

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2.1.png)

The **search** query starts with operator search (Number 1), like in a query for searching the term Login in two tables. The search result is narrowed to the last hour.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2.2.png)

All other options are incorrect.

For more information about the Azure Monitor log queries, please visit the below URLs:

- [https://docs.microsoft.com/en-us/azure/azure-monitor/logs/get-started-queries](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/get-started-queries)
- [https://docs.microsoft.com/en-us/azure/azure-monitor/logs/data-platform-logs#log-queries](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/data-platform-logs#log-queries)
- [https://docs.microsoft.com/en-us/azure/azure-monitor/logs/examples](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/examples)

Question 44 Correct

**Domain:** Implement an instrumentation strategy

Your company has just set up an Azure subscription and an Azure tenant. They are planning to set up several resources in Azure. They want to collect resource-based logs in a central location. Then the company will be able to create queries for the log data.

Which of the following could they use for the storage of resource logs?

- A. Azure Event Hubs
- B. Azure Log Analytics right
- C. Microsoft Defender for Cloud
- D. Azure Pipelines

###### Explanation:

**Correct Answer – B**

The company can direct resource logs onto a Log Analytics Workspace.

Log Analytics is a tool in the Azure portal to edit and run log queries from data collected by Azure Monitor logs and interactively analyze their results. You can use Log Analytics queries to retrieve records that match particular criteria, identify trends, analyze patterns, and provide various insights into your data.

The Microsoft documentation mentions a tutorial on the same.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/Web-capture-8-8-2023-17717-learn.microsoft.com.jpeg)

**Option A is incorrect because** Azure Event Hubs is a fully managed, real-time data ingestion service that's simple, trusted, and scalable.

**Option C is incorrect because** Microsoft Defender for Cloud is a cloud-native application protection platform (CNAPP) with a set of security measures and practices designed to protect cloud-based applications from various cyber threats and vulnerabilities.

**Option D is incorrect because** Azure Pipelines automatically builds and tests code projects.

**Reference: [Collect resource logs from an Azure resource - Azure Monitor | Microsoft Learn](https://learn.microsoft.com/en-us/azure/azure-monitor/essentials/tutorial-resource-logs)**

Question 45 Correct

**Domain:** Implement an instrumentation strategy

Your team needs to deploy a set of applications onto Azure Linux virtual machines. The application will be deployed as Docker containers. You need to send the logs emitted from the docker containers onto the Azure Monitor service. Which of the following would you install on the Azure virtual machines?

- A. Kubernetes
- B. Swarm
- C. Log Analytics Agent right
- D. Microsoft Defender for Cloud

###### Explanation:

**Correct Answer – C**

You can install the Log Analytics Agent on virtual machines. The agent would send the logs onto a Log Analytics workspace.

This is also mentioned in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_45.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

**References: [Container Monitoring solution in Azure Monitor - Azure Monitor | Microsoft Learn](https://learn.microsoft.com/en-us/previous-versions/azure/azure-monitor/containers/containers#installing-and-configuring-the-solution)**

Question 46 Correct

**Domain:** Design and implement build and release pipelines

A team wants to make use of Azure Pipelines for the continuous deployment of applications. The applications need to be deployed onto a set of Azure virtual machines.

Which of the following makes it easier to target the application release on a set of virtual machines?

- A. Agent pool
- B. Deployment groups right
- C. ARM agents
- D. Resource groups

###### Explanation:

Answer – B

You can create a deployment group and install agents on each of the servers as part of the deployment group.

This is also mentioned in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_46.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect

For more information on using deployment groups, please refer to the following link

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/release/deployment-groups/?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/deployment-groups/?view=azure-devops)

Question 47 Marked for review Incorrect

**Domain:** Implement an instrumentation strategy

You are working as Azure Data Engineer and you need to query the statements through the Log Analytics logs using Kusto Query Language(KQL) which are mainly used by users. You have to select the statements that are used in the query statements(KQL) from the given options.

- **Your Answer**
- C. Tabular expression Statement
- A. Let Statement
- D. Restrict Statement
- **Correct Answer**
- A. Let Statement
- C. Tabular expression Statement
- E. Set Statement

###### Explanation:

**Correct Answers: A, C and E**

- **Let Statement**
- **Tabular expression Statement**
- **Set Statement**

Microsoft Azure Monitor stores two types of data: logs and metrics. Azure Monitor creates a table for each log source to store its data and uses Log Analytics workspace as a data storage. You can use Azure Monitor’s Log Analytics tools or Azure Data Explorer to query logs data with the help of Kusto Query Language (KQL).

There are two types of Kusto Query Language (KQL) statements

1. User query statements – primarily used by users.
2. Application query statements — used by mid-tier applications.

Kusto Query Language defines three types of user query statements:

![](https://s3.amazonaws.com/media.whizlabs.com/learn/PT-1-Q47.png)

- **Options B and D are incorrect:** Pattern and Restrict Statements are not User query statements they are - application query statements.

**Reference:**

For more information about Kusto Query Language statement types

- [Query statements - Azure Data Explorer | Microsoft Docs](https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/statements?pivots=azuredataexplorer#user-query-statements)

Question 48 Marked for review Incorrect

**Domain:** Implement an instrumentation strategy

You are designing Azure Monitor logs deployment for a global company. You create a Log Analytics workspace and need to provide access to various teams.

What access mode type should you define for the application team?

- A. Tenant-context
- B. Workspace-context wrong
- C. Group-context
- D. Resource-context right
- E. Subscription-context

###### Explanation:

**Correct Answer: D**

When designing Azure Monitor logs deployment, you need to consider the following factors:

- The company presence — does the company need to store data in different regions or not.
- Costs of the outbound data transfers — can you keep the Azure resource data in the same region as the resources.
- The data consumption pattern — does every department in the organization require accessing their data only.

Based on the evolution of these factors, you can define the number of the required Log Analytics workspaces and their placements. You can deploy workspaces in a centralized, decentralized, or hybrid way.

The centralized deployment creates the central workspace with Azure Monitor data access management by the team or department. This is the most straightforward approach to manage the data.

The decentralized model provides workspaces for each group, and the log data is divided by resources. The data silos create difficulties for cross-team data manipulation but make data access more secure.

And the hybrid model is the parallel implementation of the models mentioned above.

Azure provides two options for workspace data access: Workspace-context and Resource-context.

When you use the Azure Monitor Logs menu, you access the data in a workspace-context mode. If you access logs within the Azure resource blade under the Monitoring section, you access the data in a resource-context mode. This mode helps you to define Azure RBAC with full granularity.

Typically, the organization’s application teams need access to the resource logs for their activities. Therefore, you need to define the resource-context type access for them.

All other options are incorrect.

For more information about Azure Monitor Logs deployment, please visit the below URLs:

- [https://docs.microsoft.com/en-us/azure/azure-monitor/logs/design-logs-deployment](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/design-logs-deployment)
- [https://docs.microsoft.com/en-us/azure/azure-monitor/logs/manage-access](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/manage-access)

Question 49 Correct

**Domain:** Develop a security and compliance plan

You integrated SonarCloud with the Azure DevOps CI pipeline. In a month, you want to see how many times SonarCloud was used.

Where can you find this information?

- A. Pipelines settings
- B. Service hooks
- C. Service connections right
- D. Agent pools

###### Explanation:

**Correct Answer: C**

Azure DevOps allows users to connect to the outside services for task execution during the pipeline run. Such tasks can be a connection to the Azure subscription, or Jenkins service for CI of the Git repos, or to SonarCloud for automatic code quality and vulnerability review. To connect to these and other services, Azure DevOps provides

Service connections.

You can create a new service connection by selecting the Service connections (Number 2) menu item on the Project Settings (Number 1) blade. You need to choose a service or a connection type from the list for the new connection and provide connection information details. After the connection is successfully created and external task execution is added to the pipeline, you can see the connection’s usage history when you open the link from the list of the Service connections. The usage history for each pipeline run will be on the Usage history tab (Number 3).

![](https://s3.amazonaws.com/media.whizlabs.com/learn/400-8.png)

- **Option A is incorrect** because the Pipelines settings menu provides parameters for retention policy and some other general settings. It does not give information about the service connections usage history.
- **Option B is incorrect** because the Service hooks menu provides subscriptions for Azure DevOps event notifications. It does not give information about the service connections usage history.
- **Option D is incorrect** because the Agent pools menu provides a pool of computing infrastructure with installed agent software to run the pipeline jobs. It does not give information about the service connections usage history.

For more information about service connections, please visit the below URLs:

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
- [https://borzenin.com/service-endpoint-usage/](https://borzenin.com/service-endpoint-usage/)

Question 50 Correct

**Domain:** Design and implement a source control strategy

Your team is planning to host a git repository using Azure Repos. The team would be hosting the following types of files-

- ASP.Net core code files
- Images, JavaScript files linked to the projects
- Audio and video files

The team wants to follow the best practices when it comes to storing the files in a git-based repository.

Which of the following can be used for managing large files such as Audio and Video files in your project?

- A. Git locking
- B. Git merge
- C. Git LFS right
- D. Git squash merge

###### Explanation:

**Answer – C**

We can use Git LFS to manage such file types. Git Large File Storage (LFS) replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.

This is also mentioned in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_50.png)

More info on Git LFS from github.com:

![](https://s3.amazonaws.com/media.whizlabs.com/learn/gitlfs.PNG)

**Option A is incorrect** because locking is not supported by Git, any developer can edit any file at any point in time. File locking is one of the features related to Git LFS which is supported by some git hosting providers. This feature helps to make sure no other developer can edit the file when it's locked.

**Option B is incorrect** because git merge is a command which is used to integrate changes from another branch.

**Option C is CORRECT** because Git LFS is used for storing large files from your source code.

**Option D is incorrect** because squash merge is a merging strategy.

For more information on working with large binary source files, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/devops/repos/git/manage-large-files?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/repos/git/manage-large-files?view=azure-devops)
- [https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage)
- [https://www.atlassian.com/git/tutorials/git-lfs](https://www.atlassian.com/git/tutorials/git-lfs)
- [https://git-lfs.github.com](https://git-lfs.github.com/)

Question 51 Correct

**Domain:** Develop a security and compliance plan

Your company is planning to use Azure DevOps. The company wants to ensure that devices can access the Azure DevOps environment. But that devices must be connected to their on-premises network. Which of the following can be used to implement this requirement?

- A. Make sure to assign Stakeholder access level to all users.
- B. Configure risky sign-ins in Microsoft Entra ID.
- C. Configure Project security in Azure DevOps.
- D. Configure conditional access in Microsoft Entra ID.right

###### Explanation:

Answer – D

You can configure conditional access to Azure Active Directory. It will ensure that only company-authenticated devices are used to access Azure-based resources.

The Microsoft documentation mentions the following on conditional access-

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_51.png)

The other options are invalid since they cannot be used to control access based on devices.

For more information on Conditional access, please refer to the following link

- [https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview)

Question 52 Correct

**Domain:** Design and implement build and release pipelines

A DevOps team is building resource manager templates that can be used to set up multiple environments in Azure. The team is making a template. This can be used to deploy an Azure SQL Server along with an Azure SQL Database on the server. A snippet of the template is given below-

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_52.1.png) ![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_52.2.png)

Which of the following would go into Slot 1?

- A. resources right
- B. child
- C. dependsOn
- D. properties

###### Explanation:

Answer – A

Here we have the child resources section for the database itself.

This is also given as an example in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_52.3.png)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on specifying resource dependency, please refer to the following link-

- [https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/define-resource-dependency](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/define-resource-dependency)

Question 53 Marked for review Incorrect

**Domain:** Design and implement build and release pipelines

Your development team is working on a microservices architecture, and you need to run end-to-end tests that require multiple test agents to simulate different user actions concurrently. Which Azure DevOps feature allows you to configure and use multiple test agents in your pipeline?

- A. Deployment Groups
- B. Microsoft-hosted Agents
- C. Self-hosted Agents right
- D. Azure DevTest Labs wrong

###### Explanation:

**Correct Answer: C**

- **Option C is CORRECT** because self-hosted agents allow you to set up and configure your agents to run on your infrastructure. This provides the flexibility to configure multiple test agents as needed to run end-to-end tests concurrently, simulating different user actions effectively.
- **Option A is INCORRECT** because deployment groups are used to define a group of target machines for deploying applications, not for configuring and using multiple test agents to run concurrent end-to-end tests.
- **Option B is INCORRECT** because Microsoft-hosted agents are managed by Microsoft and provide a predefined environment for running build and release jobs. While they can run tests, they do not provide the flexibility needed to configure and use multiple test agents specifically for simulating different user actions concurrently in a controlled manner.
- **Option D is INCORRECT** because Azure DevTest Labs is primarily used for creating and managing development and test environments in Azure. It is not designed specifically for configuring and using multiple test agents in a pipeline.

**Reference:**

- [Azure Pipelines Agents - Azure Pipelines | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/pipelines/agents/agents?view=azure-devops&tabs=yaml%2Cbrowser#self-hosted-agents)

Question 54 Correct

**Domain:** Design and implement processes and communications

You need to integrate the Azure DevOps release pipeline with ServiceNow Change Management.

The pipeline should deploy updates with ServiceNow approval of the changes.

What will you add to your pipeline to achieve your goal?

- A. Post-deployment trigger
- B. Pre-deployment approval
- C. Post-deployment gate
- D. Post-deployment approval
- E. Pre-deployment trigger
- F. Pre-deployment gate right

###### Explanation:

**Correct Answer: F**

Azure DevOps integrates with several Microsoft and third-party applications like GitHub, Jira, Teams, Slack, ServiceNow, etc.

ServiceNow is an enterprise platform that helps users with their technical management workflows. The company is focused on the management of IT services (ITMS), IT operations (ITOM), and IT business (ITBM). One of the typical integration cases between Azure DevOps and ServiceNow is an approval of CI/CD pipeline changes.

To create an approval process, you need to request the ServiceNow changes and approval. You use the **Pre-deployment gate** and add the ServiceNow Change Management extension. Before this, you must add the extension to your Azure DevOps Organization and create a service connection to ServiceNow. After changes are recorded in ServiceNow and the gate’s success state is achieved, the pipeline proceeds with the deployment, and the change request will be closed.

All other options are incorrect.

For more information about Azure DevOps and ServiceNow integration, please visit the below URLs:

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/servicenow?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/servicenow?view=azure-devops)
- [https://docs.microsoft.com/en-us/azure/devops/pipelines/release/deploy-using-approvals?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/deploy-using-approvals?view=azure-devops)

Question 55 Correct

**Domain:** Develop a security and compliance plan

You need to integrate Azure DevOps operations with ServiceNow.

What are two integration methods ServiceNow DevOps supports?

- A. RPC
- B. Webhook right
- C. ExpressRoute
- D. REST API right
- E. VPN

###### Explanation:

**Correct Answers: B and D**

Azure DevOps integrates with several Microsoft and third-party applications like GitHub, Jira, Teams, Slack, ServiceNow, etc.

ServiceNow is an enterprise platform that helps users with their technical management workflows. The company is focused on the management of IT services (ITMS), IT operations (ITOM), and IT business (ITBM). ServiceNow has its own DevOps services. The ServiceNow DevOps provides DevOps API. If needed, Azure DevOps can use direct REST API calls or Webhook notification for integration with ServiceNow DevOps.

All other options are incorrect.

For more information about Azure DevOps and ServiceNow DevOps integration, please visit the below URLs:

- [https://docs.servicenow.com/bundle/rome-devops/page/product/enterprise-dev-ops/concept/dev-ops-overview.html](https://docs.servicenow.com/bundle/rome-devops/page/product/enterprise-dev-ops/concept/dev-ops-overview.html)
- [https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/webhooks?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/service-hooks/services/webhooks?view=azure-devops)