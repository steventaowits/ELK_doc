## Elastic Cloud instance
---
For this project implementation, Elasticsearch and Kibana instance will be hosted in Elastic Cloud using Azure Cloud platform.

Two different sets of deployment, namely, _**QA**_ and _**Production**_ will be created within Elastic Cloud web platform. For starting point, each deployment uses below configurations:

|                       | ELASTICSEARCH | KIBANA        |
| :-------------------- | :------------ | :------------ |
| Memory                | 4 GB          | 1 GB          |
| Storage               | 120 GB        | N/A           |
| Fault tolerance       | 1 zone        | 1 zone        |
| Virtual Machine type  | Azure L32sv2  | Azure E32sV3  |

The configuration above can be dynamically adjusted via Elastic Cloud web platform when the need arises. 

Below information are also retrieved from Elastic Cloud web platforms: 
- Elasticsearch instance endpoint
- Kibana endpoint
- Default _elastic_ superuser credential

---
[**NEXT**: &rarr; AzDO Data Shipper Service implementation](/Documents/DesignDocument/SubFiles/DataShipperServiceImplementation.md)

[**PREVIOUS**: &larr; Elastic Stack implementation](/Documents/DesignDocument/SubFiles/ElasticStackImplementation.md)

[&larr; Table of Content](/Documents/DesignDocument/DesignDocument.md#table-of-contents)