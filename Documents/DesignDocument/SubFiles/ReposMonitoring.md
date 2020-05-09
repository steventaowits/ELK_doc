### Repos Monitoring
---

The solution covers metrics collected for Git repositories in AzDO Services, while Team Foundation Version Control (TFVC) repository metrics are not included in the solution. However, the solution will check the existence of TFVC repository within the AzDO Services.

Collected data and its Azure reference links:

- [List of repository in a team project](https://docs.microsoft.com/en-us/rest/api/azure/devops/git/repositories/list?view=azure-devops-rest-5.1)
- [List of all branches and its statistics within a repository](https://docs.microsoft.com/en-us/rest/api/azure/devops/git/stats/list?view=azure-devops-rest-5.1)
- [List of policy configurations in a repo / branch](https://docs.microsoft.com/en-us/rest/api/azure/devops/git/policy%20configurations/get?view=azure-devops-rest-5.1)
- [Get a list of Tfvc items](https://docs.microsoft.com/en-us/rest/api/azure/devops/tfvc/items/list?view=azure-devops-rest-5.1)

**Visualization Dashboard**

The Repos. monitoring dashboard contains the following metrics.

| Data  | Kibana Visualization Type  |
| --- | --- |
| Last Updated Time | Metric |
| Total # of Repository  | Metric  |
| List of all Repos  | Data Table  |
| Repos. Size List | Horizontal Bar |
| Repos. Size Trend | Line |
| [Branch Policy] Ratio # of master branches with policy vs without policy  | Pie  |
| [Branch Policy] List of branches without branch policy  | Data Table  |
| [Branch Policy] List of branches with branch policy  | Data Table  |
| [Branch Policy] List of branches with min. reviewer policy and its setting  | Data Table  |
| [Branch Policy] List of branches with merge strategy | Data Table |
| [Branch Policy] List of branches with comments requirements | Data Table |
| [Branch Policy] List of branches with linked work items check | Data Table |
| Ratio # of active vs stale branches  | Pie  |
| List of stale branches  | Data Table  |
| Total # of Branches vs Repository vs Project   | Pie |
| Total # of TFVC Repository  | Metric  |
| List of TFVC Repository | Data Table  |

---
[**NEXT**: &rarr; Elastic Stack implementation](/Documents/DesignDocument/SubFiles/ElasticStackImplementation.md)

[**PREVIOUS**: &larr; Overview Monitoring](/Documents/DesignDocument/SubFiles/OverviewMonitoring.md)

[&larr; Table of Content](/Documents/DesignDocument/DesignDocument.md#table-of-contents)