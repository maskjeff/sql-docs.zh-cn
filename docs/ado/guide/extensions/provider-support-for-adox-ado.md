---
description: ADOX 的提供程序支持 (ADO)
title: 提供程序支持 ADOX (ADO) |Microsoft Docs
ms.prod: sql
ms.prod_service: connectivity
ms.technology: ado
ms.custom: ''
ms.date: 01/19/2017
ms.reviewer: ''
ms.topic: conceptual
helpviewer_keywords:
- ADOX provider support [ADO]
ms.assetid: 64234ce5-dc46-4c8a-a316-61956b6b9abb
author: rothja
ms.author: jroth
ms.openlocfilehash: cbc2b4821ac5c57c2302892caff1afa742e829b9
ms.sourcegitcommit: 18a98ea6a30d448aa6195e10ea2413be7e837e94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2020
ms.locfileid: "88978688"
---
# <a name="provider-support-for-adox-ado"></a>ADOX 的提供程序支持 (ADO)
ADOX 的某些功能不受支持，具体取决于 OLE DB 的数据访问接口。 [Microsoft Jet 的 OLE DB 提供程序](../appendixes/microsoft-ole-db-provider-for-microsoft-jet.md)完全支持 ADOX。 下表列出了 [用于 SQL Server 的 microsoft OLE DB 提供程序](../appendixes/microsoft-ole-db-provider-for-sql-server.md)、适用于 [ODBC 的 Microsoft OLE DB 提供程序](../appendixes/microsoft-ole-db-provider-for-odbc.md)或 [Oracle 的 Microsoft OLE DB 提供程序](../appendixes/microsoft-ole-db-provider-for-oracle.md) 的不支持的功能。 任何其他 Microsoft OLE DB 提供程序都不支持 ADOX。  
  
## <a name="microsoft-ole-db-provider-for-sql-server"></a>Microsoft OLE DB Provider for SQL Server  
  
|对象或集合|使用限制|  
|--------------------------|-----------------------|  
|**表** 集合|属性在对象创建之前是可读/写的，并且在引用现有对象时为只读。|  
|**视图** 集合|不支持**视图**。|  
|**过程** 集合|不支持 **Append** 和 **Delete** 方法。|  
|**Procedure** 对象|不支持 **命令** 属性。|  
|**键** 集合|不支持 **Append** 和 **Delete** 方法。|  
|**用户** 集合|**用户** 不受支持。|  
|**组** 集合|不支持**组**。|  
  
## <a name="microsoft-ole-db-provider-for-odbc"></a>Microsoft OLE DB Provider for ODBC  
  
|对象或集合|使用限制|  
|--------------------------|-----------------------|  
|**目录** 对象|**Create**方法不受支持。|  
|**表** 集合|不支持 **Append** 和 **Delete** 方法。 属性在对象创建之前是可读/写的，并且在引用现有对象时为只读。|  
|**过程** 集合|不支持 **Append** 和 **Delete** 方法。|  
|**Procedure** 对象|不支持 **命令** 属性。|  
|**索引** 集合|不支持 **Append** 和 **Delete** 方法。|  
|**键** 集合|不支持 **Append** 和 **Delete** 方法。|  
|**用户** 集合|**用户** 不受支持。|  
|**组** 集合|不支持**组**。|  
  
## <a name="microsoft-ole-db-provider-for-oracle"></a>Microsoft OLE DB Provider for Oracle  
  
|对象或集合|使用限制|  
|--------------------------|-----------------------|  
|**目录** 对象|**Create**方法不受支持。|  
|**表** 集合|不支持 **Append** 和 **Delete** 方法。 属性在对象创建之前是可读/写的，并且在引用现有对象时为只读。|  
|**视图** 集合|不支持 **Append** 和 **Delete** 方法。|  
|**查看** 对象|不支持 **命令** 属性。|  
|**过程** 对象|不支持 **Append** 和 **Delete** 方法。|  
|**Procedure** 对象|不支持 **命令** 属性。|  
|**索引** 集合|不支持 **Append** 和 **Delete** 方法。|  
|**键** 集合|不支持 **Append** 和 **Delete** 方法。|  
|**用户** 集合|**用户** 不受支持。|  
|**组** 集合|不支持**组**。|