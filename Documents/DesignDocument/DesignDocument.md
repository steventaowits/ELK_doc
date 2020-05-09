# Table of Content
---

- [Overview](#overview)
    - [Problem Statement](#problem-statement)
    - [Proposed Solution](#proposed-solution)
    - [Design Principles](#design-principles)
- [Elastic Stack Planning](SubFiles/ElasticStackPlanning.md)
    - [AzDO Services Monitoring](SubFiles/ElasticStackPlanning.md#azdo-services-monitoring)
        - [Overview Monitoring](SubFiles/OverviewMonitoring.md)
        - [Repos Monitoring](SubFiles/ReposMonitoring.md)
- [Elastic Stack implementation](SubFiles/ElasticStackImplementation.md)
    - [Elastic Cloud instance](SubFiles/ElasticCloudInstance.md)
    - [AzDO Data Shipper Services](SubFiles/DataShipperServiceImplementation.md)
    - [Logstash](SubFiles/LogstashImplementation.md)
    - [Continous Integration & Continous Delivery](SubFiles/AzurePipelinesImplementation.md)
- [References](SubFiles/ElasticReferences.md)


# Overview
---

This document serves as the AVEVA Elastic Stack project implementation design reference for project stakeholders. This is a living document, which will be continuously updated to reflect the latest design implementation. This document shall also serve as the source of truth in the occurrence of any dispute within any stage of the project.

## Problem Statement

As a large enterprise with hundreds of projects and teams across the board, utilizing various public cloud services and on-prem infrastructures, and also working collaboratively to embrace DevOps culture, AVEVA is in need for a centralized solution to:

- monitor and measure the effectiveness of each team DevOps implementation.
- monitor public cloud services resource usage efficiency.
- monitor on-prem infrastructures resource health and usage efficiency.
- receive alerts for operational critical information.

## Proposed Solution

The solution proposes a centralized web platform to provide meaningful visualization of various metrics stated previously. The solution utilizes Elastic Stack by Elastic company at its core with various data input sources, including, but not limited to Azure DevOps (AzDO) Services metrics, public cloud resources and on-prem infrastructure metrics and logs. Some custom software will be developed to fill in the gap of features not readily available within Elastic Stack offerings, such as the data collection and shipper for AzDO Services metrics.

## Design Principles

The proposed solution covers below items as its design principles

- **High-availability**

The solution shall utilize public cloud to leverage its high-availability standard. Elastic Cloud is chosen as the Elastic Stack platform with at least two availability zones hosted in separate data center region to achieve high-availability and provide data redundancy. Metrics and logs data should also periodically backed up for an extra level of redundancy. Custom developed software will also run on Azure Cloud platform.

- **Extensible**

The design shall consider future expansion possibility to integrate more input sources and others output module. For example, Grafana can be used as an alternative of Kibana for metrics visualization.

- **Secure**

The solution uses secure communication exchange between its entire components. For AzDO Services Monitoring, the solution shall consider the threat analysis modelling from Microsoft Threat Modelling Tool and provide mitigation approach.

- **Scalable**

The solution should be able to scale from small deployment to enterprise level deployment without sacrificing its performance. Elastic Cloud provides user-friendly interface to scale the deployment configuration dynamically.

- **Modular**

The solution shall utilize modularity for all its features whenever possible, so that features can be newly added or removed from the solution without affecting other features.


---
[**NEXT**: &rarr; Elastic Stack Planning](/Documents/DesignDocument/SubFiles/ElasticStackPlanning.md)