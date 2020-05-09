## Continuous Integration &amp; Continuous Delivery
---

Azure Pipelines facilitates CI &amp; CD processes for this project. YAML pipelines are used and mainly divided into these categories:

| Pipeline | Output | Remarks |
| --- | --- | --- |
| Azure Resource creation & env. setup | Azure Function App, Logstash ACI, Azure Key Vault, Azure Managed Identity. Each of these Azure Resources will have 2 sets: QA and Prod. | This pipeline creates all the Azure Cloud Resources to be used for this project. It also ingest the necessary secrets into Key Vaults to be used by other YAML pipelines. |
| Data Shipper Service | Data Shipper Service artifacts | This pipeline deploys the Data Shipper Service build artifacts to the designated Azure Function App. |
| Logstash Configurations | Logstash configuration files in Azure Storage account | This pipeline deploys the Logstash configuration files into Azure Storage account. |
| Kibana deployment | Kibana Space, Dashboard, User Role, and User | This pipeline creates Kibana Space with visualization dashboard and user with read-only permission to the space. |

For details of Azure Pipeline's configuration, its prerequisites, and how to modify it, please refer to _Deployment Guide_.

In general, the release pipeline workflow is illustrated below.

![elastic_azure_pipelines](Images/elastic_azure_pipelines.jpg)

| **Note:** The implementation above includes QA env. deployment as a placeholder for future implementation. Test report should be published after QA env. deployment, which will be referenced by the project owner as one of consideration to proceed with Prod. env. deployment. |
| --- |

---
[**PREVIOUS**: &larr; Logstash implementation](/Documents/DesignDocument/SubFiles/LogstashImplementation.md)

[&larr; Table of Content](/Documents/DesignDocument/DesignDocument.md#table-of-contents)