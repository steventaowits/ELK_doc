### Overview Monitoring
---

The overview monitoring covers metrics at the Organization level, such as the total number of Projects, Teams, and Members across the entire AVEVA AzDO Organization.

Collected data and its Azure REST API reference links:

- [List of all projects within Organization ](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-5.1)
- [List of all teams within Project](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get%20teams?view=azure-devops-rest-5.1)
- [List of all members within Organization ](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get%20team%20members%20with%20extended%20properties?view=azure-devops-rest-5.1)

**Visualization Dashboard**

The Overview monitoring dashboard contains the following metrics.

| Data  | Kibana Visualization Type  |
| --- | --- |
| Last Updated Time | Metric |
| Total # of Projects  | Metric  |
| Total # of Teams  | Metric  |
| Total # of Members  | Metric  |
| List of all Projects  | Data Table  |
| List of all Teams  | Data Table  |
| List of all Members  | Data Table  |

---
[**NEXT**: &rarr;  Repos Monitoring](/Documents/DesignDocument/SubFiles/ReposMonitoring.md)

[**PREVIOUS**: &larr; Elastic Stack planning](/Documents/DesignDocument/SubFiles/ElasticStackPlanning.md)

[&larr; Table of Content](/Documents/DesignDocument/DesignDocument.md#table-of-contents)