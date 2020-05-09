# Elastic Stack Implementation
---

This section describes the low-level design details. For details on the project resources setup and implementation, please refer to _Developer Guide_.

Below table summarizes the components and its platform service for existing implementation.

| Components | Platform service |
| --- | --- |
| Kibana | Elastic Cloud (Azure) |
| Elasticsearch | Elastic Cloud (Azure) |
| Logstash | Azure Container Instance |
| Data Shipper Service | Azure Function App |

Sub-sequent sections describes each implementation in more details manner.

---
[**NEXT**: &rarr;  Elastic Cloud instance implementation](/Documents/DesignDocument/SubFiles/ElasticCloudInstance.md)

[**PREVIOUS**: &larr; Repos Monitoring](/Documents/DesignDocument/SubFiles/ReposMonitoring.md)

[&larr; Table of Content](/Documents/DesignDocument/DesignDocument.md#table-of-contents)