---
title: Release Burndown
titleSuffix: Azure DevOps Server
description: Learn how to build a report that shows how quickly your team has delivered backlog items and track how much work the team must still do to complete a product release.
ms.technology: devops-analytics
ms.topic: reference
ms.assetid: 9044206f-c993-451d-bcc8-6f3980c90b3e
ms.author: kaelli
author: KathrynEE
ms.date: 10/15/2021
---


# Release Burndown

[!INCLUDE [version-lt-azure-devops](../../includes/version-lt-azure-devops.md)]

By reviewing the Release Burndown report, you can understand how quickly your team has delivered backlog items and track how much work the team must still do to complete a product release.  
  
> [!NOTE]
>  This report requires that the team project collection that contains your team project was provisioned with SQL Server Reporting Services. This report is not available if ![Report](media/icon_reportte.png "Icon_reportTE") **Reports** does not appear when you open Azure DevOps and expand your team project node.  
  
## Prerequisites  
  
 To view the report, you must be assigned or belong to a group that has been assigned the **Browser** role in Reporting Services. For more information, see [Grant permissions to view or create reports in Azure DevOps Server](../admin/grant-permissions-to-reports.md).  

<a name="Data"></a>

## Data in the report

 As the following illustration shows, a Release Burndown graph shows how much work remained at the start of each sprint in a release. The source of the raw data is your product backlog. Each sprint that has been assigned to the team project or team appears along the horizontal axis. The vertical axis indicates the sum of all effort of all active backlog items at the start of each sprint. As the team updates the state of backlog items to Done, the effort remaining goes down. The amount of estimated effort on the vertical axis is in whatever unit that your scrum team has decided to use (for example, story points, size, or hours).  
  
 ![Release burndown chart](media/scrum_releaseburndonw.png "Scrum_ReleaseBurndonw")  
  
 You can filter the report by selecting the **Release Path** or **Area**.  
  
### Required activities for tracking release burndown  

For the burndown graph to be useful and correct, your team must carry out the following activities for tracking work items:  
  
-   Specify the number of releases you want to track and [define the start and end dates for each sprint](../../boards/sprints/define-sprints.md).  
  
-   Define product backlog items and bugs, and assign each to a sprint or iteration.  (**Iteration** field). Make sure that all backlog items are assigned to your team's area path or subarea.  
  
-   At the start of a release, estimate the **Effort** for each product backlog item and each bug that your team will work on.  
  
-   During the sprint or at the close of each sprint, for each product backlog item and each bug that the team completed, change the **State** to **Done**.  

<a name="Interpreting"></a>

## Interpreting the report  

You can review the report to determine the progress that your team has made in a release and to answer the following questions:  
  
-   How much work remains in the release?  
  
-   How quickly is your team working through the product backlog?  
  
## Related articles 

[Scrum process](../../boards/work-items/guidance/scrum-process.md)
[Define area paths](../../organizations/settings/set-area-paths.md) or [Define iteration paths](../../organizations/settings/set-iteration-paths-sprints.md)