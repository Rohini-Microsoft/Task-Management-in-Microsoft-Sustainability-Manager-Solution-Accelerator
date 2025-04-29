# Task Management in Microsoft Sustainability Manager (MSM) 

The Task Management in Microsoft Sustainability Manager (MSM) accelerator enhances MSM by enabling users to manage tasks within a single interface. This accelerator facilitates task creation, assignment, collaboration, and resolution, improving productivity and visibility, and ensuring timely completion of sustainability-related tasks.

<br/>

<div align="center">
  
[**SOLUTION OVERVIEW**](#solution-overview)  \| [**QUICK DEPLOY**](#quick-deploy)  \| [**BUSINESS USE CASE**](#business-use-case)  \| [**SUPPORTING DOCUMENTATION**](#supporting-documentation)

</div>
<br/>

<h2><img src="./Deployment/images/readme/solution-overview.png" width="48" />
Solution overview
</h2>

This solution accelerator enhances the efficiency of Microsoft Sustainability Manager by adding the ability to effortlessly create, assign, manage, and track tasks. Following the same UI, UX and architecture of MSM, this accelerator introduces a task table having custom N:1 relationships with multiple MSM tables so users (Sustainability Managers, Analysts and other personas) can create, assign, track and manage tasks. The accelerator also has 2 custom security roles so managers can create & assign tasks throughout the organization whereas Analysts would be able to view, create & edit tasks assigned to them. Additionally, there will be notifications sent out in Microsoft Teams and Outlook upon task creation through Power Automate.

### Solution architecture

Below diagram depicts the architecture of this solution accelerator. 

![image](./Deployment/images/readme/architecture.png)

### How to customize - Do not have content
If you'd like to customize the solution accelerator, here are some common areas to start:

{🟨TODO: Fill in links to supplementary documentations}

[Doc name](./docs/...)

[Doc name](./docs/...)

[Doc name](./docs/...)

<br/>

### Additional resources - Do not have content

{🟨TODO: Fill in links to other internal or external links}

[Doc name]()

[Doc name]()

<br/>

### Key features
<details open>
  <summary>Click to learn more about the key features this solution enables</summary>

  - **Task Creation and assignment** <br/>
  The ability to quickly create tasks, related to the use of MSM, and assign them to team members in the same tool, MSM, that will be used to resolve the tasks according to security roles.  
    
  - **Progress tracking** <br/>
  Visualization of progress, status, and dates enables rapid and clear monitoring to ensure tasks are on track to meet deadlines. This helps in identifying any delays or bottlenecks early.
  
  - **Notifications and reminders** <br/>
  Automated notifications help ensure that team members are aware of upcoming deadlines, task assignments. This feature reduces the need for frequent follow-ups and keeps everyone aligned.
  
  - **Custom security roles** <br/>
  Customizable security roles to grant and limit visibility to view and edit tasks based on persona.  This ensures the Sustainability Manager can view all tasks and Sustainability Analysts can view only their own tasks. 
  
  - **Collaboration and communication** <br/>
  Built-in collaboration with comments and real-time updates within tasks allows the assigner to provide additional context, answer questions, and ensure that everyone involved has the information they need to complete the tasks effectively.
    
</details>

<br /><br />
<h2><img src="./Deployment/images/readme/quick-deploy.png" width="48" />
Quick deploy
</h2>

### How to install or deploy
Please click this [**Link to Deployment Guide**](./Deployment/README.md) for instructions on how to deploy and set up the solution accelerator. 

{🟨TODO: Remove if Azure OpenAI quota check is not required }

> ⚠️ **Important: Check Azure OpenAI Quota Availability - Do not have content**
 <br/>To ensure sufficient quota is available in your subscription, please follow [quota check instructions guide](./docs/QuotaCheck.md) before you deploy the solution.

<br/>

### Prerequisites and Costs - Do not have content
{🟨TODO: Update with solution specific notes like role requirements}

To deploy this solution accelerator, ensure you have access to an [Azure subscription](https://azure.microsoft.com/free/) with the necessary permissions to create **resource groups, resources, app registrations, and assign roles at the resource group level**. This should include Contributor role at the subscription level and  Role Based Access Control role on the subscription and/or resource group level. Follow the steps in [Azure Account Set Up](./docs/AzureAccountSetUp.md).

Here are some example regions where the services are available: {🟨TODO: Update with suggested regions specific to this solution}

Check the [Azure Products by Region](https://azure.microsoft.com/en-us/explore/global-infrastructure/products-by-region/?products=all&regions=all) page and select a **region** where the following services are available.

{🟨TODO: Call out specific pricing "gotchas" like Azure Container Registry if known}

Pricing varies per region and usage, so it isn't possible to predict exact costs for your usage. The majority of the Azure resources used in this infrastructure are on usage-based pricing tiers. However, Azure Container Registry has a fixed cost per registry per day.

{🟨TODO: Update with solution specific estimate sheet}

Use the [Azure pricing calculator](https://azure.microsoft.com/en-us/pricing/calculator) to calculate the cost of this solution in your subscription. 

Review a [sample pricing sheet](https://azure.com/e/68b51f4cb79a4466b631a11aa57e9c16) in the event you want to customize and scale usage.

_Note: This is not meant to outline all costs as selected SKUs, scaled use, customizations, and integrations into your own tenant can affect the total consumption of this sample solution. The sample pricing sheet is meant to give you a starting point to customize the estimate for your specific needs._

<br/>

{🟨TODO: Update with all products, decription of product use, and product specific pricing links}

| Product | Description | Cost |
|---|---|---|
| [Product Name with Link to Learn content](https://learn.microsoft.com) | Decription of how the product is used | [Pricing]() |
| [Product Name with Link to Learn content](https://learn.microsoft.com) | Decription of how the product is used | [Pricing]() |
| [Product Name with Link to Learn content](https://learn.microsoft.com) | Decription of how the product is used | [Pricing]() |
| [Product Name with Link to Learn content](https://learn.microsoft.com) | Decription of how the product is used | [Pricing]() |


<br/>

>⚠️ **Important:** To avoid unnecessary costs, remember to take down your app if it's no longer in use,
either by deleting the resource group in the Portal or running `azd down`.

<br /><br />
<h2><img src="./Deployment/images/readme/business-scenario.png" width="48" />
Business Use Case
</h2>

Below is a sample landing page of the solution accelerator after it is deployed, set up, and ready to be used.

![Landing Page](./Deployment/images/readme/landingPage.png)

As a Sustainability Manager or Sustainability Analyst, you will be able to deploy this accelerator on top of your existing MSM environment. This will allow you to
 1. Create, manage, track, and assign tasks as a Sustainability Manager specific to MSM tables like Emissions, Scope 1, Scope 2 and Scope 3 activity tables, Accounts etc. You can create generic tasks for data validation, data import, etc. This also allows you to get a 360 view of all scheduled, completed and in-progress tasks to help you to prioritize, delegate, and track progress.
 2. As a Analyst, you will receive notifications when a task is assigned to the user. There will be custom views to track & manage tasks assigned to the logged in user. 

### Business value - Added new
<details>
  <summary>Click to learn more about what value this solution provides</summary>

  - **Increased productivity** <br/>
  A single solution saves time switching between tools and makes it easier to manage and track tasks.

  - **Clearer visibility** <br/>
  A single solution provides a clear overview of all tasks, making it secure, easier to prioritize, and monitor progress
     
</details>

<br /><br />
<h2><img src="./Deployment/images/readme/supporting-documentation.png" width="48" />
Supporting documentation
</h2>

Please refer to following additional documentation along with [Microsoft Sustainability Manager(MSM)](https://learn.microsoft.com/en-us/industry/sustainability/sustainability-manager-overview):

1. [Microsoft Teams](https://learn.microsoft.com/en-us/microsoftteams/) 
2. [Microsoft Power Automate](https://learn.microsoft.com/en-us/power-automate/) 
3. [Model Driven Apps in Power Apps](https://learn.microsoft.com/en-us/power-apps/maker/model-driven-apps)
4. [Microsoft Dataverse](https://learn.microsoft.com/en-us/power-apps/maker/data-platform/)

### Security guidelines - Do not have content

{🟨TODO: Fill in with solution specific security guidelines similar to the below}

This template uses Azure Key Vault to store all connections to communicate between resources.

This template also uses [Managed Identity](https://learn.microsoft.com/entra/identity/managed-identities-azure-resources/overview) for local development and deployment.

To ensure continued best practices in your own repository, we recommend that anyone creating solutions based on our templates ensure that the [Github secret scanning](https://docs.github.com/code-security/secret-scanning/about-secret-scanning) setting is enabled.

You may want to consider additional security measures, such as:

* Enabling Microsoft Defender for Cloud to [secure your Azure resources](https://learn.microsoft.com/azure/security-center/defender-for-cloud).
* Protecting the Azure Container Apps instance with a [firewall](https://learn.microsoft.com/azure/container-apps/waf-app-gateway) and/or [Virtual Network](https://learn.microsoft.com/azure/container-apps/networking?tabs=workload-profiles-env%2Cazure-cli).

<br/>

### Frequently asked questions - Do not have content

{🟨TODO: Remove this section if you don't have FAQs}

[Click here](./docs/FAQs.md) to learn more about common questions about this solution.

<br/>

### Cross references - Do not have content
Check out similar solution accelerators
 
{🟨TODO: Identify related accelerators - fill in the name and a one sentence description. The name should have non-breaking spaces in them to make sure the layout doesn't break.}

| Solution Accelerator | Description |
|---|---|
| [Document&nbsp;knowledge&nbsp;mining](https://github.com/microsoft/Document-Knowledge-Mining-Solution-Accelerator) | Provides REST API access to OpenAI's powerful language models including o3-mini, o1, o1-mini, GPT-4o, GPT-4o mini |
| [Conversation&nbsp;knowledge&nbsp;mining](https://github.com/microsoft/Conversation-Knowledge-Mining-Solution-Accelerator) | Description of solution accelerator |
| [Document&nbsp;generation](https://github.com/microsoft/document-generation-solution-accelerator) | Analyzes various media content—such as audio, video, text, and images—transforming it into structured, searchable data |


<br/>   


## Provide feedback - do not have content

{🟨TODO: Update link to create new issues for this repo}

Have questions, find a bug, or want to request a feature? [Submit a new issue](https://github.com/microsoft/content-processing-solution-acclerator/issues) on this repo and we'll connect.

<br/>

## Responsible AI Transparency FAQ - Do not have content
Please refer to [Transparency FAQ](./TRANSPARENCY_FAQ.md) for responsible AI transparency details of this solution accelerator.

<br/>

## Disclaimers

This release only supports English language input and output. Users should not attempt to use the system with any other language or format. The system output may not be compatible with any translation tools or services, and may lose its meaning or coherence if translated. 

This release does not reflect the opinions, views, or values of Microsoft Corporation or any of its affiliates, subsidiaries, or partners. The system output is solely based on the system's own logic and algorithms, and does not represent any endorsement, recommendation, or advice from Microsoft or any other entity. Microsoft disclaims any liability or responsibility for any damages, losses, or harms arising from the use of this release or its output by any user or third party. 

This release does not provide any financial advice, and is not designed to replace the role of qualified client advisors in appropriately advising clients. Users should not use the system output for any financial decisions or transactions, and should consult with a professional financial advisor before taking any action based on the system output. Microsoft is not a financial institution or a fiduciary, and does not offer any financial products or services through this release or its output. 

This release is intended as a proof of concept only, and is not a finished or polished product. It is not intended for commercial use or distribution, and is subject to change or discontinuation without notice. Any planned deployment of this release or its output should include comprehensive testing and evaluation to ensure it is fit for purpose and meets the user's requirements and expectations. Microsoft does not guarantee the quality, performance, reliability, or availability of this release or its output, and does not provide any warranty or support for it. 

This Software requires the use of third-party components which are governed by separate proprietary or open-source licenses as identified below, and you must comply with the terms of each applicable license in order to use the Software. You acknowledge and agree that this license does not grant you a license or other right to use any such third-party proprietary or open-source components.  

To the extent that the Software includes components or code used in or derived from Microsoft products or services, including without limitation Microsoft Azure Services (collectively, “Microsoft Products and Services”), you must also comply with the Product Terms applicable to such Microsoft Products and Services. You acknowledge and agree that the license governing the Software does not grant you a license or other right to use Microsoft Products and Services. Nothing in the license or this ReadMe file will serve to supersede, amend, terminate or modify any terms in the Product Terms for any Microsoft Products and Services. 

You must also comply with all domestic and international export laws and regulations that apply to the Software, which include restrictions on destinations, end users, and end use. For further information on export restrictions, visit https://aka.ms/exporting. 

You acknowledge that the Software and Microsoft Products and Services (1) are not designed, intended or made available as a medical device(s), and (2) are not designed or intended to be a substitute for professional medical advice, diagnosis, treatment, or judgment and should not be used to replace or as a substitute for professional medical advice, diagnosis, treatment, or judgment. Customer is solely responsible for displaying and/or obtaining appropriate consents, warnings, disclaimers, and acknowledgements to end users of Customer’s implementation of the Online Services. 

You acknowledge the Software is not subject to SOC 1 and SOC 2 compliance audits. No Microsoft technology, nor any of its component technologies, including the Software, is intended or made available as a substitute for the professional advice, opinion, or judgement of a certified financial services professional. Do not use the Software to replace, substitute, or provide professional financial advice or judgment.  

BY ACCESSING OR USING THE SOFTWARE, YOU ACKNOWLEDGE THAT THE SOFTWARE IS NOT DESIGNED OR INTENDED TO SUPPORT ANY USE IN WHICH A SERVICE INTERRUPTION, DEFECT, ERROR, OR OTHER FAILURE OF THE SOFTWARE COULD RESULT IN THE DEATH OR SERIOUS BODILY INJURY OF ANY PERSON OR IN PHYSICAL OR ENVIRONMENTAL DAMAGE (COLLECTIVELY, “HIGH-RISK USE”), AND THAT YOU WILL ENSURE THAT, IN THE EVENT OF ANY INTERRUPTION, DEFECT, ERROR, OR OTHER FAILURE OF THE SOFTWARE, THE SAFETY OF PEOPLE, PROPERTY, AND THE ENVIRONMENT ARE NOT REDUCED BELOW A LEVEL THAT IS REASONABLY, APPROPRIATE, AND LEGAL, WHETHER IN GENERAL OR IN A SPECIFIC INDUSTRY. BY ACCESSING THE SOFTWARE, YOU FURTHER ACKNOWLEDGE THAT YOUR HIGH-RISK USE OF THE SOFTWARE IS AT YOUR OWN RISK.