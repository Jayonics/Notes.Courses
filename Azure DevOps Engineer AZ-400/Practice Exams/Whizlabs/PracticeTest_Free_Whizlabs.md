---
title: "LMS | Whizlabs"
source: "https://www.whizlabs.com/learn/course/microsoft-azure-certification-az-400/270/quiz/60704/report/8328003"
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
| 1 | Develop a security and compliance plan | 5 | 3 | 2 | 0 | 1 |
| 2 | Design and implement a source control strategy | 2 | 2 | 0 | 0 | 0 |
| 3 | Design and implement build and release pipelines | 7 | 6 | 1 | 0 | 1 |
| 4 | Implement an instrumentation strategy | 2 | 2 | 0 | 0 | 1 |
| 5 | Design and implement processes and communications | 4 | 3 | 1 | 0 | 2 |
| Total | All Domains | 20 | 16 | 4 | 0 | 5 |

Question 1 Correct

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

Question 2 Correct

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

Question 3 Correct

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

Question 4 Incorrect

**Domain:** Design and implement build and release pipelines

A company wants to deploy a web-based application onto Azure. The application is going to be hosted on a set of Azure virtual machines located in different regions. They want to implement a strategy of Blue-Green deployment for all future application updates. You also want to implement an Azure DNS load balancing solution to implement Blue-Green deployments.

Which of the following would be implemented as a feature to enable Blue-Green Deployments?

- A. Automatic updates
- B. Rolling updates
- C. Weighted round-robin routing method right
- D. Priority routing method wrong

###### Explanation:

**Answer – C**

When you are implementing the Azure Traffic Manager as the DNS routing service, you can use the Weighted round-robin routing method for implementing Blue-Green deployments.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/26/ckeditor_41.png)

**Option A is incorrect** because, with automatic updates, all endpoints will be updated to the latest version either at the same time or after a small gap which is against the blue-green deployment.

**Option B is incorrect** because there is no environment isolation between the old and new application versions in a rolling deployment.

**Option C is CORRECT** because the Weighted round-robin routing method is used for achieving blue-green deployment with Azure Traffic Manager.

**Option D is incorrect** because in the case of the priority routing method we have a primary service endpoint for all traffic, so it is not possible to have two versions of the application at a point in time and all traffic will always be routed to the endpoint with the highest priority.

For more information on the article itself, please refer to the following link-

- [https://azure.microsoft.com/en-in/blog/blue-green-deployments-using-azure-traffic-manager](https://azure.microsoft.com/en-in/blog/blue-green-deployments-using-azure-traffic-manager)

Question 5 Correct

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

Question 6 Marked for review Incorrect

**Domain:** Develop a security and compliance plan View Case Study  

Which of the following access level would you provide for the whizlab-developers group?

- A. Reader right
- B. Collaborator
- C. Contributor wrong
- D. Owner

###### Explanation:

**Answer – A**

In the case studies we have the following information

\------------------------

- Packages that are required by the application during the development phase will be installed by members of a group called whizlab-developers

\---------------------------.

This means the member of "whizlab-developers" group need to install the application hence we need to give "Reader" role only

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/10/15/ckeditor_111_29_28.png)

**Option A is CORRECT** because with the reader role developers will get permission to install the packages as per the requirement in question.

**Option B is incorrect** because as per the requirement we need to assign permissions based on the principle of least privilege. With the Collaborator role, developers will get permission to save packages from upstream sources which is not specified in the requirement.

**Option C is incorrect** because as per the requirement we need to assign permissions based on the principle of least privilege. With the Contributor role, developers will get permission to publish, unlist, and promote packages to a view as well that are not specified in the requirement.

**Option D is incorrect** because as per the requirement we need to assign permissions based on the principle of least privilege. With the Owner role, developers will get all permissions that are not required as per the requirement.

For more information on sharing and securing packages, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/devops/artifacts/feeds/feed-permissions?view=azure-devops#feed-permissions-overview](https://docs.microsoft.com/en-us/azure/devops/artifacts/feeds/feed-permissions?view=azure-devops#feed-permissions-overview)

Question 7 Correct

**Domain:** Develop a security and compliance plan

A team is developing an application that would be deployed using ARM templates. The templates would also be used to create virtual machines. You need to store a secret for the virtual machine in an Azure Key Vault.

You need to complete the following script for this purpose.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2019/06/20/ckeditor_azure_400_pt2-q48_2_49_11.jpg)

Which of the following would go into Slot3?

- A. keyvault
- B. vault
- C. secret right
- D. set

###### Explanation:

**Answer - C**

An example of this is given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/az-400-2-23.JPG)

Since this is clearly mentioned in the Microsoft documentation, all other options are incorrect.

For more information on creating a key vault via the CLI, please visit the below URL-

- [https://docs.microsoft.com/en-us/azure/key-vault/secrets/quick-create-cli#add-a-secret-to-key-vault](https://docs.microsoft.com/en-us/azure/key-vault/secrets/quick-create-cli#add-a-secret-to-key-vault)

Question 8 Correct

**Domain:** Design and implement build and release pipelines

Your team currently has an Azure DevOps project and an Azure subscription. The subscription contains an Azure SQL database named whizlabdb. They want to create a release pipeline. It would use the Azure SQL Database deployment task to update the database. Which of the following should they use as an artifact in the update process?

- A. BACPAC file
- B. DACPAC file right
- C. LDF file
- D. MDF file

###### Explanation:

**Answer – B**

You can use a DACPAC file for scheme related changes.

The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/29/ckeditor_32.png)

**Option A is incorrect** because the primary use case for a BACPAC is to move a database from one server to another or to migrate a database from a local server to the cloud and archive an existing database in an open format. It's not used for performing schema-related changes in an existing database.

**Option B is CORRECT** because the DACPAC file is used for packaging and deploying schema-related changes in the release pipeline.

**Option C is incorrect** because the main purpose of using the LDF file in SQL Server is to roll back the database in case of data loss.

**Option D is incorrect** because the MDF file is a Master Database File used by Microsoft SQL Server to store user data and not for deploying the schema changes.

For more information on Azure SQL database deployment, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/targets/azure-sqldb?view=azure-devops&tabs=yaml](https://docs.microsoft.com/en-us/azure/devops/pipelines/targets/azure-sqldb?view=azure-devops&tabs=yaml)
- [https://docs.microsoft.com/en-us/sql/relational-databases/data-tier-applications/data-tier-applications?view=sql-server-ver16](https://docs.microsoft.com/en-us/sql/relational-databases/data-tier-applications/data-tier-applications?view=sql-server-ver16)

Question 9 Correct

**Domain:** Develop a security and compliance plan

Your team needs to deploy several Azure Resource Manager templates. These templates will refer to secrets stored in the Azure Key Vault service. You have to recommend the right solution. It will access to the secrets in the Key Vault during the deployment of the Azure Resource Manager templates. You have to ensure the solution that uses the principle of least privilege.

Which of the following would you use to restrict access to delete the key vault?

- A. Azure Key vault access policy
- B. A Personal Access Token
- C. OAuth 2.0
- D. RBAC right

###### Explanation:

**Answer – D**

For control plane access to the key vault, you can use Role-based access control.

The Microsoft documentation mentions the following.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/29/ckeditor_42.png)

**Option A is incorrect** because with the Azure Key Vault access policy you can manage secrets, keys, and certificates. You do not get control plane level access, so you can not delete the key vault.

**Option B is incorrect** because you can use a personal access token (PAT) as an alternate password to authenticate into Azure DevOps but it can not be used for deleting azure resources.

**Option C is incorrect** because OAuth2.0 is the industry-standard protocol for authorization, it does not provide user permission to delete the key vault. For delete permissions, we need to use RBAC.

**Option D is CORRECT** because with RBAC you can assign user permission for the control plane where the user can modify and delete the key vault.

For more information on securing the Key Vault, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/key-vault/general/secure-your-key-vault](https://docs.microsoft.com/en-us/azure/key-vault/general/secure-your-key-vault)
- [https://docs.microsoft.com/en-us/azure/key-vault/general/rbac-guide?tabs=azure-cli](https://docs.microsoft.com/en-us/azure/key-vault/general/rbac-guide?tabs=azure-cli)

Question 10 Correct

**Domain:** Design and implement build and release pipelines

A team is planning to use Azure DevOps for managing the build and release pipelines for their applications. The key requirements for change requests and approvals in the build process are given below.

- There is a set of users that must manually validate a change request and approve the deployment onto a stage.
- It needs to be ensured that no active issues are present in a work item before deployment of a build onto a stage.
- It needs to be ensured that no active incidents are present in the system after it has been deployed and before promoting the release.
- During the deployment pipeline, you have to prompt the user to enter the value for a parameter that will be used on certain deployment tasks.

Which of the following is the feature to use for the requirement?

**“It needs to be ensured that no active issues are present in a work item before deployment of a build onto a stage.”**

- A. Pre-deployment approvals
- B. Post-deployment approvals
- C. Pre-deployment gates right
- D. Post-deployment gates
- E. Manual Intervention

###### Explanation:

**Answer – C**

Here we have to use Pre-deployment gates.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/29/ckeditor_52.png)

Since this is clearly given in the Microsoft documentation, all **other** **options are incorrect**.

For more information on Azure Pipelines release gates and approvals, please visit the following URL-

- [https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/approvals/?view=azure-devops)

Question 11 Correct

**Domain:** Design and implement processes and communications

A company is currently planning to use the Azure DevOps service for managing the CI/CD pipeline for various applications. The team wants to have an effective communication tool that can be used across the project. The tool should integrate with Azure DevOps and also have a separation of channels for each team.  
You decide to implement Bamboo.  
Does this fulfill the requirement?

- A. Yes
- B. No right

###### Explanation:

**Answer – B**

Bamboo is a continuous integration server offered by Atlassian. Bamboo allows you to automate the release management of a software application, creating a continuous delivery.

This is not a communication tool. For communication, we can use tools like Slack or Microsoft Teams.

For more information on the Bamboo tool, please visit the below URL-

- [https://www.atlassian.com/software/bamboo](https://www.atlassian.com/software/bamboo)
- [https://confluence.atlassian.com/bamboo/understanding-the-bamboo-ci-server-289277285.html](https://confluence.atlassian.com/bamboo/understanding-the-bamboo-ci-server-289277285.html)

Question 12 Correct

**Domain:** Design and implement build and release pipelines

A company wants to follow the Azure DevOps strategy for its development and deployment process. They want to ensure that during the development phase the following requirements are taken care of:

- Scanning of 3rd party packages in the code base for vulnerabilities
- Checking for unlicensed libraries in the code base

The company decides to implement these checks as part of the Continuous Integration process.

Would this fulfill the requirement?

- A. Yes right
- B. No

###### Explanation:

**Answer – A**

For both the requirements, we need to perform a Software Composition Analysis (SCA) scan. This scan should be part of the Continuous Integration process to check these vulnerabilities.

The Microsoft documentation mentions the following representation on the CI/CD pipeline.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/30/ckeditor_26.png)

For more information on software composition analysis in the CI/CD pipeline, please visit the following URL-

- [https://docs.microsoft.com/en-us/learn/modules/software-composition-analysis/3-explore-software-composition-analysis](https://docs.microsoft.com/en-us/learn/modules/software-composition-analysis/3-explore-software-composition-analysis)
- [https://docs.microsoft.com/en-us/learn/modules/software-composition-analysis/6-integrate-software-composition-analysis-checks-into-pipelines](https://docs.microsoft.com/en-us/learn/modules/software-composition-analysis/6-integrate-software-composition-analysis-checks-into-pipelines)

Question 13 Marked for review Correct

**Domain:** Design and implement build and release pipelines

A company is planning on using Azure DevOps. They want to use DevOps practices for the development and deployment of applications. They have the following requirements for Build pipeline automation and they want to implement the requirements for different development teams.

- “Ensure that only code that compiles and passes unit testing is checked into the Integration branch.”
- “Ensure that code is of good quality before it is released to the test area.”
- “Ensure that security vulnerabilities are identified as soon as possible in the code base.”

Which of the following technique in build automation can be used for the following requirement?

**“Ensure code is of good quality before it is released to the test area.”**

- A. Daily Builds
- B. Gated Check-ins
- C. Code Analysis Integrations right
- D. Fortify Integrations

###### Explanation:

**Answer – C**

You can accomplish this with Code Analysis Integrations.

This is also given in the Microsoft documentation.

![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/06/30/ckeditor_48.png)

**Option A is incorrect** because daily builds will build the code but won't check for any code quality issues.

**Option B is incorrect** because gated check-in is a process that restricts developers from merging a broken code into the source control system, it does not perform any code quality scan.

**Option C is CORRECT** because, for code quality check, Code Analysis needs to be automated in the build pipeline.

**Option D is incorrect** because Fortify integration is used for security vulnerability scanning and not for code quality.

For more information on code analysis, please visit the following URL-

- [https://www.perforce.com/blog/kw/static-analysis-ci-cd-pipelines](https://www.perforce.com/blog/kw/static-analysis-ci-cd-pipelines)

Question 14 Incorrect

**Domain:** Develop a security and compliance plan

A company currently has the following resources defined as part of its Azure subscription.

- Windows Server 2019 container images that are stored in Azure Container Registry
- A Log Analytics workspace
- Azure virtual machines that run the latest version of Ubuntu
- An Azure Key vault

For which of the following would you receive security vulnerability assessments? Choose two answers from the options given below.

- A. Windows Server 2019 container images that are stored in Azure Container Registry right
- B. The Log Analytics workspace
- C. Azure virtual machines that run the latest version of Ubuntu wrong
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

Question 15 Correct

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

Question 16 Marked for review Correct

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

Question 17 Marked for review Incorrect

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

- A. Agile wrong
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

Question 18 Correct

**Domain:** Design and implement processes and communications

Whizlabs decided to integrate the GitHub repository with Azure Boards for their Azure DevOps web application project.

Which group-members can make such a connection regarding permissions?

Please select two answers.

- A. GitHub Collaborator and DevOps Project Administrators
- B. GitHub Owner and DevOps Project Contributors right
- C. GitHub Collaborator and DevOps Project Contributors
- D. GitHub Owner and DevOps Project Endpoint Administrators
- E. GitHub Owner and DevOps Project Administrators right

###### Explanation:

Correct Answers: B and E

Only GitHub repository or organization Owner and members of Azure DevOps Project Administrators or Project Contributors groups can make a connection between GitHub Repository and Azure Boards.

**![](https://s3.amazonaws.com/media.whizlabs.com/learn/2020/08/10/ckeditor_4.png)**

Option A is incorrect since the GitHub repository Collaborator does not have permission to create a connection.

Option C is incorrect since the GitHub repository Collaborator does not have permission to create a connection.

Option D is incorrect since members of DevOps Project Endpoint Administrators do not have permission to create a connection.

For more information about GitHub repository and Azure Boards integration, please visit the below URLs-

- [https://docs.microsoft.com/en-us/azure/devops/boards/github/connect-to-github?view=azure-devops](https://docs.microsoft.com/en-us/azure/devops/boards/github/connect-to-github?view=azure-devops)
- [https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/permission-levels-for-a-user-account-repository#collaborator-access-on-a-repository-owned-by-a-user-account](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/permission-levels-for-a-user-account-repository#collaborator-access-on-a-repository-owned-by-a-user-account)

Question 19 Marked for review Correct

**Domain:** Implement an instrumentation strategy

You are configuring Azure Resource logs for Azure functions in your company to get detailed diagnostic and auditing information for each function. It would help if you analyzed the logs using powerful log queries and visualizations. You configured the diagnostic settings to send the logs to the Log Analytics workspace.

Now you have an additional requirement to send the logs outside of Azure. Which are the actions you need to perform to achieve this? Choose two.

- A. Add a new diagnostic setting for the Function App and select ‘Stream to an event hub’.right
- B. From the diagnostic settings of the Function App select ‘Archive to a storage account'.
- C. From the diagnostic settings of the Function App deselect ‘Send to Log Analytics’.
- D. Create an event hub from the Azure Portal.right
- E. From the Log Analytics workspace, modify Log management settings.

###### Explanation:

**Correct Answers: A and D**

- **Option A is** **correct.** As the requirement is to send logs outside of Azure, the event hub should be selected as a destination for the logs. For this, a new setting should be created. This can be configured from the monitoring section of the function app. Each resource can have up to 5 diagnostic settings.
- **Option B is** **incorrect.** Archive to a storage account option can be used in case you want to store logs in a storage account but it can not be used for sending logs outside of azure.
- **Option C is** **incorrect.** An azure resource can send logs to more than one destination type. You can configure a different diagnostic setting to send logs to the event hub. And at the same time, you can maintain the existing diagnostic setting and keep sending the logs to the Log Analytics workspace. And as it is a requirement to analyze the logs using queries and visualization, it is required to send the logs to the Log Analytics workspace.
- **Option D is** **correct.** An event hub must be created to receive the logs from the function app and to send the logs outside of Azure. Resource logs from event hubs are consumed in JSON format with a records element containing the records in each payload and can be consumed by any third-party SIEM or other log analytics solutions.
- **Option E is** **incorrect.** Log management is used for storing the logs from different Azure resources. For example, the logs from the function app will be stored under the ‘FunctionAppLogs’ table in the Log management of the Log Analytics workspace. There is no provision to send logs outside of Azure.

**Reference:**  
For more information on configuring the log framework in Azure, please refer to the below link

- [https://docs.microsoft.com/en-us/azure/azure-monitor/platform/platform-logs-overview](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/platform-logs-overview)

Question 20 Correct

**Domain:** Implement an instrumentation strategy

You enabled distributed tracing for an application using the native capabilities of Application Insights. One of the components, say component A, receives a request from the browser and calls another component, say component B, using HTTP.

You analyzed the resulting telemetry in Application insights, which displayed three telemetries. A request telemetry from component A with ID ‘ARID’, parent id ‘PARID’ and root operation id ‘OAID’; A dependency telemetry from component A with ID ‘ADID’ and a request telemetry from component B with ID ‘BRID.’

What should be the Parent id of the only dependency telemetry?

- A. PARID
- B. ARID right
- C. OAID
- D. BRID

###### Explanation:

**Answer: B**

- **Option A is incorrect.** The parent id denotes the id of the parent telemetry. In this scenario, the request telemetry from component A is the parent telemetry of component A’s dependency telemetry. ‘PARID’ is the parent id of component A’s request telemetry, which will not be reused anywhere else in operation.
- **Option B is** **correct.** ‘ARID’ is the id of component A’s request telemetry. This will be used as a parent Id of the dependency telemetry. This ensures the correlation between the telemetries. To clarify the telemetries, componentA receives the request from the browser and sends it to component B. For component A, it receives a request, then sends it to B, which means a request telemetry and a dependency telemetry are required. Component B receives a call from A. Hence only the request telemetry is required.
- **Option C is incorrect.** ‘OAID’ is the unique id for the correlation. To associate telemetry with a logical operation, every telemetry item has a context field called ‘operation\_Id’. This identifier is shared by every telemetry item in the distributed trace. So even if you lose telemetry from a single layer, you can still associate telemetry reported by other components.
- **Option D is incorrect.** ‘BRID’ is the request id of component B’s request telemetry. This is initiated by the dependency call from component A and uses its id, which is ‘ADID’ as its parent Id.
- **Reference Link:** For more information on distributed tracing and telemetry correlation, please refer to the below link from Microsoft- [https://docs.microsoft.com/en-us/azure/azure-monitor/app/distributed-tracing](https://docs.microsoft.com/en-us/azure/azure-monitor/app/distributed-tracing),[https://docs.microsoft.com/en-us/azure/azure-monitor/app/correlation](https://docs.microsoft.com/en-us/azure/azure-monitor/app/correlation)