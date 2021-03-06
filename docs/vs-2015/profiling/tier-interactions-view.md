---
title: "Tier Interactions View | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "vs.performance.view.tierinteraction"
helpviewer_keywords: 
  - "Tier Interactions view"
ms.assetid: bb4fb21c-f3f7-473a-8b5e-442da4c2c445
caps.latest.revision: 20
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# Tier Interactions View
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

The latest version of this topic can be found at [Tier Interactions View](https://docs.microsoft.com/visualstudio/profiling/tier-interactions-view).  
  
Tier interaction profiling provides additional information about the execution times in functions of multitiered applications that communicate with databases through [!INCLUDE[vstecado](../includes/vstecado-md.md)]. Data is collected only for synchronous function calls.  
  
 **Requirements**  
  
-   [!INCLUDE[vsUltLong](../includes/vsultlong-md.md)]  
  
 The Interactions View displays tier interaction data in two panes:  
  
-   The master pane is a hierarchical tree. The top level row contains aggregated data for the database connections of an [!INCLUDE[vstecasp](../includes/vstecasp-md.md)] page or a process. Child nodes contain aggregated data for the database connections of the parent.  
  
-   When you click a database call node in the master pane, data for the instance of the database call is displayed in the details pane.  
  
 Time is displayed as the number of milliseconds or the number of CPU clock ticks. To change the time unit displayed, click the **Tools** menu, click **Options**, and then choose one of the **Show time values as** options.  
  
## Master Pane  
  
|Column|Description|  
|------------|-----------------|  
|**Name**|-   For a top level row, the name of the profiled process or Web page.<br />-   For a database connection row, the name of the server that hosts the database.|  
|**Database**|The name of the database (database connection rows only).|  
|**Count**|The total number of requests that are generated by the process, Web page, or database connection.|  
|**Total Elapsed Time**|The total time that is spent executing any one request from the process, Web page, or database connection.|  
|**Max Elapsed Time**|The maximum time spent executing any one request from the process, Web page, or database connection.|  
|**Min Elapsed Time**|The minimum time that is spent executing any one request from the process, Web page, or database connection.|  
|**Avg Elapsed Time**|The average time that is spent executing a request from the process, Web page, or database connection.|  
  
## Database Connection Details Pane  
  
|Column|Description|  
|------------|-----------------|  
|**Command Text**|The SQL query of the request.|  
|**Query Count**|The number of times the query was run.|  
|**Total Elapsed Time**|The total time that is spent executing the instances of the query.|  
|**Max Elapsed Time**|The maximum time that is spent executing any one instance of the query.|  
|**Min Elapsed Time**|The minimum time that is spent executing any one instance of the query.|  
|**Avg Elapsed Time**|The average time that is spent executing an instance of the query.|



