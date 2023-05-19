# langchain-bot-ansible

## Set up Secrets and Variables

### Secrets

AZURE_CREDENTIALS: Follow [https://learn.microsoft.com/en-us/azure-stack/user/ci-cd-github-action-login-cli?view=azs-2301](https://learn.microsoft.com/en-us/azure-stack/user/ci-cd-github-action-login-cli?view=azs-2301#get-service-principal)
```
az ad sp create-for-rbac --name "myApp" --role contributor `
    --scopes /subscriptions/{subscription-id}/resourceGroups/{resource-group} `
    --sdk-auth
```

SSH_USER: Your preferred SSH username

SSH_PASSWORD: Your preferred SSH password

### Variables

VM_NAME: Name of Azure Resource Group and VM

LOCATION: Azure VM Location



## Run the GitHub Actions

Goto Actions -> Azure VM Deployment -> Run workflow
