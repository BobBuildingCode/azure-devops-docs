---
title: Run Coverage tables 
titleSuffix: Azure DevOps Server
description: Learn how to use FactRunCoverage to query for data in Azure DevOps Server.
ms.technology: devops-analytics
ms.topic: reference
ms.assetid: 4868da2c-9402-444e-a4a4-6b99e71a27ac
ms.author: kaelli
author: KathrynEE
ms.date: 10/19/2021
---


# Run Coverage tables

[!INCLUDE [version-lt-azure-devops](../../includes/version-lt-azure-devops.md)]

Use FactRunCoverage and the associated dimensions to query for data. Find out how thoroughly a particular test run covered the code that it was intended to test.

For information about the measures and dimensions that are associated with these tables in the SQL Server Analysis Services cube, see [Code churn and code coverage](perspective-code-analyze-report-code-churn-coverage.md).  
  
![Fact Table for Run Coverage](media/teamproj_factruncoverage.png "TeamProj_FactRunCoverage")  
  
> [!NOTE]
>  You cannot aggregate these coverage values to determine code coverage for a build. To determine the code coverage in a build, you must use FactBuildCoverage. For more information, see [Build Coverage tables](table-reference-build-coverage.md).  
  
FactRunCoverage is associated with the following dimension tables:
  
- DimAssembly
- DimBuild
- DimBuildFlavor
- DimBuildPlatform
- DimDate  
- DimPerson
- DimTestRun
  
For more information, see these articles:
- [Code churn and code coverage](perspective-code-analyze-report-code-churn-coverage.md)   
- [Code Churn](/previous-versions/azure/devops/report/excel/code-coverage-excel-report)  
- [Build](/visualstudio/ide/walkthrough-building-an-application)   
- [Table reference for the relational warehouse database](table-reference-relational-warehouse-database.md)
