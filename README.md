# Load  Files from Jira  into CogSearch 
### The issues from Jira are loaded into CogSearch by following below steps
- Establish a connection with Jira using the Python SDK.
- Retrieve the required issues from Jira using the JQL query and Search method.
- Use Azure open ai to index the issue content.
- Index the parsed chunks into Azure Cognitive Search.
- Repeat the process for all the required files.

#### Using the Azure Storage Pyhon SDK  to fetch the file stream and use PYPDF and Document Intelligence to chunk the page in memory and create a vector index
- https://developer.atlassian.com/cloud/jira/platform/rest/v3/api-group-issue-search/#api-rest-api-3-search-post
- Refer to https://github.com/MSUSAzureAccelerators/Azure-Cognitive-Search-Azure-OpenAI-Accelerator/blob/main/04-Complex-Docs.ipynb for loading large documents using PYPDF and Document Intelligence- 
