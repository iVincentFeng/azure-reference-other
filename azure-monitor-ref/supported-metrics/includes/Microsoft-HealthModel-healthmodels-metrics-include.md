---
ms.service: azure-monitor
ms.topic: include
ms.date: 09/19/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.HealthModel/healthmodels, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|Query execution duration<p><p>Overall duration of executing all configured queries in parallel and calculating the model health state. |`ExecutionDuration` |Milliseconds |Average, Minimum, Maximum |No Dimensions|PT1M |Yes|
|Health score per node<p><p>Health score per node in the model. Dimension splitting should be applied. Can be a value between 0 and 100 percent. Update frequency depends on the refreshInterval of the health model. Does not include the root node. |`NodeHealthScore` |Percent |Average, Minimum, Maximum |NodeName|PT1M |Yes|
|Overall health score<p><p>The health score of the root node represents the overall health of the model. Can be a value between 0 and 100 percent. Update frequency depends on the refreshInterval of the health model. |`OverallHealthScore` |Percent |Average, Minimum, Maximum |No Dimensions|PT1M |Yes|