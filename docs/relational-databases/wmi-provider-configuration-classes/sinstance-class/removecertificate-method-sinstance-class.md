---
description: "RemoveCertificate Method (SInstance Class)"
title: "RemoveCertificate Method (SInstance)"
ms.custom: seo-lt-2019
ms.date: "03/14/2017"
ms.service: sql
ms.reviewer: ""
ms.subservice: wmi
ms.topic: "reference"
apiname: 
  - "RemoveCertificate Method (SInstance Class)"
apilocation: 
  - "sqlmgmproviderxpsp2up.mof"
apitype: "MOFDef"
helpviewer_keywords: 
  - "RemoveCertificate method"
ms.assetid: 7e5dbafa-a634-4617-9622-510514fce0ce
author: markingmyname
ms.author: maghan
---
# RemoveCertificate Method (SInstance Class)
[!INCLUDE [SQL Server](../../../includes/applies-to-version/sqlserver.md)]
  Removes the current security certificate from the instance of [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)].  
  
## Syntax  
  
```  
  
object.RemoveCertificate()  
```  
  
## Parts  
 *object*  
 An [SInstance Class](../../../relational-databases/wmi-provider-configuration-classes/sinstance-class/sinstance-class.md) object that represents the server settings on an instance of [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)].  
  
## Property Value/Return Value  
 A uint32 value, which is 0 if the service was successfully modified, 1 if the request is not supported, and any other number to indicate an error.  
  
## Remarks  
  
## See Also  
 [Configuring Server Network Protocols and Net-Libraries](https://msdn.microsoft.com/library/ms177485\(v=sql.100\).aspx)  
  
  
