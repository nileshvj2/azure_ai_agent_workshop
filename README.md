# azure_ai_agent_workshop
Azure AI Agent service hands on workshop (Internal)

## Set up

1. You need to have below resources set up in Azure: 

    * Azure AI Foundry Hub and Project
    * Azure AI Foundry connections (using key or Entra authentication)
        * Azure Open AI service
        * Azure AI search service 
    * Deploy gpt 4o-mini (or any gpt model of your choice)
    * Deploy text-embedding-ada-002 
    * Azure AI search index created 

    *Pls refer previous workshop set up instructions, if needed - nileshvj2/AzureAIFoundry_Workshop*

2. Set up service principal using Azure Entra ID
    * Create service principal "svc-aifoundry-user" in Azure Entra ID and provide below permissions
        * *"Azure AI Developer"* permission at the resource group level
        * *"Cognitive services Open AI user"* permission at the resource group level
    
3. Rename *credentials.txt* file to *credentials.env* file 

4. For svc-aifoundry-user - add AZURE_TENANT_ID, AZURE_CLIENT_ID and AZURE_CLIENT_SECRET in the credentials.env file

5. Provide all other required config values in the *credentials.env*
