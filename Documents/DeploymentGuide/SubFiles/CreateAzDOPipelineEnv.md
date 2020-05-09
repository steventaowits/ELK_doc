# Create AzDO Pipelines Environment
---

The AzDO Pipeline environment is currently only used for enabling manual approval gateway before deploying the solution to Production environment.

1. In your AzDO web portal, navigate to your Project &rarr; **Pipelines** &rarr; **Environments**
2. Click _New environment_ on the top right corner
3. Fill in below information:

   - _Name_ : "Elastic-QA-environment"
   - _Resource_ : _None_

4. Click _Create_
5. Repeat above steps for Production environment with below info:

   - _Name_ : "Elastic-Prod-environment"
   - _Resource_ : _None_

6. After the environments have been created successfully, then follow [this guide](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/approvals?view=azure-devops&tabs=check-pass#approvals) to add the manual approval members.

---
[**NEXT**: &rarr; AzDO Pipeline creation](CreateAzDOPipelines.md)

[**PREVIOUS**: &larr; Create AzDO Variable groups](CreateAzDOVariableGroups.md)

[&larr; Table of Content](/Documents/DeploymentGuide/DeploymentGuide.md)