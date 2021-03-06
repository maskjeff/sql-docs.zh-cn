---
description: ATN2 (Transact-SQL)
title: ATN2 (Transact-SQL) | Microsoft Docs
ms.custom: ''
ms.date: 07/24/2017
ms.prod: sql
ms.prod_service: database-engine, sql-database, sql-data-warehouse, pdw
ms.reviewer: ''
ms.technology: t-sql
ms.topic: language-reference
f1_keywords:
- ATN2
- ATN2_TSQL
dev_langs:
- TSQL
helpviewer_keywords:
- arctangent
- tangent
- ATN2 function
ms.assetid: 014b291e-7cd7-4c39-b20d-5db3a9f0505d
author: markingmyname
ms.author: maghan
monikerRange: '>=aps-pdw-2016||=azuresqldb-current||=azure-sqldw-latest||>=sql-server-2016||=sqlallproducts-allversions||>=sql-server-linux-2017||=azuresqldb-mi-current'
ms.openlocfilehash: 7dd9d89534be641da25c0cbf0d4f7e1e58d82dde
ms.sourcegitcommit: cc23d8646041336d119b74bf239a6ac305ff3d31
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "91117137"
---
# <a name="atn2-transact-sql"></a>ATN2 (Transact-SQL)
[!INCLUDE [sql-asdb-asdbmi-asa-pdw](../../includes/applies-to-version/sql-asdb-asdbmi-asa-pdw.md)]

返回以弧度表示的角，该角位于正 X 轴和原点至点 (y, x) 的射线之间，其中 x 和 y 是两个指定的浮点表达式的值。
  
![主题链接图标](../../database-engine/configure-windows/media/topic-link.gif "“主题链接”图标") [Transact-SQL 语法约定](../../t-sql/language-elements/transact-sql-syntax-conventions-transact-sql.md)
  
## <a name="syntax"></a>语法  
  
```syntaxsql
ATN2 ( float_expression , float_expression )  
```  
  
[!INCLUDE[sql-server-tsql-previous-offline-documentation](../../includes/sql-server-tsql-previous-offline-documentation.md)]

## <a name="arguments"></a>参数
*float_expression*  
float 数据类型的[表达式](../../t-sql/language-elements/expressions-transact-sql.md)****。
  
## <a name="return-types"></a>返回类型
**float**
  
## <a name="examples"></a>示例  
以下示例计算指定的 `ATN2` 向量和 `x` 向量的 `y`。
  
```sql
DECLARE @x FLOAT = 35.175643, @y FLOAT = 129.44;  
SELECT 'The ATN2 of the angle is: ' + CONVERT(VARCHAR, ATN2(@y, @x));  
GO  
```  
  
[!INCLUDE[ssResult](../../includes/ssresult-md.md)]
  
```
The ATN2 of the angle is: 1.30545                         
(1 row(s) affected)  
```  
  
## <a name="see-also"></a>另请参阅
[CAST 和 CONVERT (Transact-SQL)](../../t-sql/functions/cast-and-convert-transact-sql.md)  
[float 和 real (Transact-SQL)](../../t-sql/data-types/float-and-real-transact-sql.md)  
[数学函数 (Transact-SQL)](../../t-sql/functions/mathematical-functions-transact-sql.md)
  
  

