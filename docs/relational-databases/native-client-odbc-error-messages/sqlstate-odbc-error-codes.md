---
title: SQLSTATE (ODBC 错误代码) |Microsoft Docs
description: 当 SQL Server ODBC 驱动程序将存储过程作为远程存储过程运行时，该过程可以具有整数返回代码和输出参数。
ms.custom: ''
ms.date: 03/14/2017
ms.prod: sql
ms.prod_service: database-engine, sql-database, sql-data-warehouse, pdw
ms.reviewer: ''
ms.technology: native-client
ms.topic: reference
helpviewer_keywords:
- SQL Server Native Client ODBC driver, errors
- ODBC error handling, cause information
- messages [ODBC], cause information
- SQLSTATEs
- errors [ODBC], cause information
ms.assetid: 84cce528-edb0-473f-a85f-3eb87fbe2cf3
author: markingmyname
ms.author: maghan
monikerRange: '>=aps-pdw-2016||=azuresqldb-current||=azure-sqldw-latest||>=sql-server-2016||=sqlallproducts-allversions||>=sql-server-linux-2017||=azuresqldb-mi-current'
ms.openlocfilehash: a358a3cd071c3b0a986925a1ef5fc181536283c0
ms.sourcegitcommit: 4d370399f6f142e25075b3714e5c2ce056b1bfd0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "91868325"
---
# <a name="sqlstate-odbc-error-codes"></a>SQLSTATE（ODBC 错误代码）
[!INCLUDE[SQL Server Azure SQL Database Synapse Analytics PDW ](../../includes/applies-to-version/sql-asdb-asdbmi-asa-pdw.md)]

  SQLSTATE 提供与警告或错误的原因有关的详细信息。 对于在检测并返回的数据源中发生的错误 [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] ， [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] NATIVE Client ODBC 驱动程序将返回的本机错误号映射到相应的 SQLSTATE。 如果本机错误号没有要映射到的 ODBC 错误代码，则 [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] Native CLIENT ODBC 驱动程序将返回 SQLSTATE 42000 ( "语法错误或访问冲突" ) 。 对于驱动程序检测到的错误， [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] Native CLIENT ODBC 驱动程序将生成相应的 SQLSTATE。  
  
 有关状态错误代码的详细信息，请参阅下面的主题：  
  
-   [附录 A：ODBC 错误代码](../../odbc/reference/appendixes/appendix-a-odbc-error-codes.md)  
  
-   [SQLSTATE 映射](../../odbc/reference/develop-app/sqlstate-mappings.md)  
  
## <a name="see-also"></a>另请参阅  
 [处理错误和消息](../../relational-databases/native-client-odbc-error-messages/handling-errors-and-messages.md)  
  
