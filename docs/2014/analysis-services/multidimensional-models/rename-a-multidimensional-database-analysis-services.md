---
title: "Rename a Multidimensional Database (Analysis Services) | Microsoft Docs"
ms.custom: ""
ms.date: "06/13/2017"
ms.prod: "sql-server-2014"
ms.reviewer: ""
ms.technology: "analysis-services"
ms.topic: conceptual
helpviewer_keywords: 
  - "renaming databases"
ms.assetid: 15fdaec7-f3e4-44d9-9b78-1a1d78c484e0
author: minewiskan
ms.author: owend
---
# Rename a Multidimensional Database (Analysis Services)
  The manner in which you change the name of a [!INCLUDE[msCoName](../../includes/msconame-md.md)] [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] database depends upon how you connect to the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] database. To change the name of an existing database, you must connect in online mode. To change the name of the database into which objects in an [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] project will be instantiated, you must connect in project mode.  
  
### To change the database name in online mode  
  
1.  Using [!INCLUDE[ssBIDevStudio](../../includes/ssbidevstudio-md.md)], connect directly to the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] database.  
  
2.  In Solution Explorer, right-click the database and then click **Edit Database**.  
  
3.  In the **Database name** text box, change the database name.  
  
4.  Click **Save** or **Save All** on the toolbar, click **Save Selected Items** or **Save All** on the **File** menu, or close the **Database Designer** and then click **Save** when prompted.  
  
     The database name is updated in the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] instance and the database object in Solution Explorer is refreshed.  
  
### To change the database name in project mode  
  
1.  Open the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] project.  
  
2.  In Solution Explorer, right-click the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] project and then click **Properties**.  
  
3.  In the **Property Pages** dialog box, click **Deployment** in the **Configuration Properties** section.  
  
4.  Change the **Database** property to the new database name.  
  
     The next time the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] project is deployed, it will be deployed to this new database name. If this database already exists, it will be overwritten.  
  
### To change the database name using SQL Server Management Studio  
  
-   Right-click the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] database and edit the Name property.  
  
## See Also  
 [Configure Server Properties in Analysis Services](../server-properties/server-properties-in-analysis-services.md)   
 [Set Multidimensional Database Properties &#40;Analysis Services&#41;](set-multidimensional-database-properties-analysis-services.md)   
 [Configure Analysis Services Project Properties &#40;SSDT&#41;](configure-analysis-services-project-properties-ssdt.md)   
 [Deploy Analysis Services Projects &#40;SSDT&#41;](deploy-analysis-services-projects-ssdt.md)  
  
  
