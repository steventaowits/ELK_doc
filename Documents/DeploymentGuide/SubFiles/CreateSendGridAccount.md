# Create SendGrid account
---

SendGrid account is required for sending error notification emails. Follow below steps for creating SendGrid account:

1. Download the Powershell scripts from repository to your local machine: _/Pipeline/Prerequisites_
2. In your local machine, open Powershell ISE &rarr; navigate to the scripts path
3. Execute "_DeploySendGrid.ps1_"

   `.\DeploySendGrid.ps1`

4. Fill in the _SendGrid account_, _Azure Resource Group name_, and _password_ at the prompt
5. Once SendGrid account has been provisioned successfully, get the the _username_ generated from the terminal

   ![SendGrid username](Images/SendGrid_username.png)

6. Login to [SendGrid](https://app.sendgrid.com/) by _username_ and _password_ you created earlier.
7. Follow the guide [here](https://docs.microsoft.com/en-us/azure/sendgrid-dotnet-how-to-send-email#to-find-your-sendgrid-api-key) to retrieve SendGrid API key.

   > Note: You will need to input the SendGrid API key into _SetupData.ps1_ for setting up the AzDO Variable groups.

---
[**NEXT**: &rarr; Create AzDO Variable groups](CreateAzDOVariableGroups.md)

[**PREVIOUS**: &larr; Create new AzDO Service connection](AzDOServiceConnection.md)

[&larr; Table of Content](/Documents/DeploymentGuide/DeploymentGuide.md)