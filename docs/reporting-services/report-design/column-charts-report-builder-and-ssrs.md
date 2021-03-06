---
title: 柱形图（报表生成器）| Microsoft Docs
description: 在报表生成器中通过柱形图显示一段时间内的比较或数据更改。 将序列显示为一组按类别分组的垂直图条。
ms.date: 03/03/2017
ms.prod: reporting-services
ms.prod_service: reporting-services-native
ms.technology: report-design
ms.topic: conceptual
ms.assetid: ae8c138b-e356-4ad8-862c-a4a8d0c04149
author: maggiesMSFT
ms.author: maggies
ms.openlocfilehash: 8973b80e17b2c6bbedcdd7140fa87148c64d6538
ms.sourcegitcommit: 5c7634b007f6808c87094174b80376cb20545d5f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2020
ms.locfileid: "84881955"
---
# <a name="column-charts-report-builder-and-ssrs"></a>柱形图（报表生成器和 SSRS）
  柱形图将序列显示为一组按类别分组的垂直图条。 柱形图对于显示一段时间的数据变化或说明各项之间的比较来说十分有用。 平面柱形图与条形图关系密切，条形图将序列显示为多组水平图条，而范围柱形图将序列显示为多组具有不同起点和终点的垂直图条。 有关详细信息，请参阅 [条形图（报表生成器和 SSRS）](../../reporting-services/report-design/bar-charts-report-builder-and-ssrs.md) 和 [范围图（报表生成器和 SSRS）](../../reporting-services/report-design/range-charts-report-builder-and-ssrs.md)。  
  
 柱形图非常适用于此数据，因为所有这三个序列都共享一个公共时间段，允许进行有效比较。  
  
> [!NOTE]  
>  [!INCLUDE[ssRBRDDup](../../includes/ssrbrddup-md.md)]  
  
## <a name="variations-of-a-column-chart"></a>柱形图变体  
  
-   **堆积**。 一种多个序列垂直堆积的柱形图。 如果图表中只有一个序列，则堆积柱形图将与柱形图的显示相同。  
  
-   **百分比堆积**。 一种多个序列垂直堆积以占满图表区的柱形图。 如果图表中只有一个序列，则所有柱形条将占满图表区。  
  
-   **三维簇状**。 一种将每个序列分别显示在三维图表的单独行中的柱形图。  
  
-   **三维圆柱**。 一种图条在三维图表中的形状类似于圆柱的柱形图。  
  
-   **直方图**。 一种图表通过计算以使其图条按正态分布进行排列的柱形图。  
  
-   **排列图**。 一种图条按从最高到最低排列的柱形图。  
  
## <a name="data-considerations-for-a-column-chart"></a>柱形图在数据方面的注意事项  
  
-   条形图和柱形图最常用于说明各组之间的比较情况。 如果图表中存在三个以上的序列，请考虑使用堆积条形图或柱形图。 如果图表中有多个序列，则还可以将堆积条形图或柱形图收集到多个组中。 有关详细信息，请参阅 [条形图（报表生成器和 SSRS）](../../reporting-services/report-design/bar-charts-report-builder-and-ssrs.md)。  
  
-   在柱形图中，在以水平方式显示类别轴标签时空间会很局促。 如果类别标签较长，请考虑使用条形图或更改标签的旋转角度。  
  
-   您可以在柱形图中为单个图条添加特殊的绘制样式以增加其视觉效果。 绘制样式包括楔形、浮雕、圆柱形和由明到暗。 设计这些效果的目的是为了改进二维图表的外观。 即使使用的是三维图表，您仍可应用绘制样式，但效果可能不会相同。 有关如何向条形图添加绘制样式的详细信息，请参阅 [向图表添加凹凸效果、阳文和纹理样式（报表生成器和 SSRS）](../../reporting-services/report-design/chart-effects-add-bevel-emboss-or-texture-report-builder.md)。  
  
-   柱形图的独特功能是将图表显示为直方图或排列图。 为此，可在“属性”窗口中将 **Histogram** 或 **Pareto** 的 ShowColumnAs 属性设置为 **true**。  
  
## <a name="see-also"></a>另请参阅  
 [图表（报表生成器和 SSRS）](../../reporting-services/report-design/charts-report-builder-and-ssrs.md)   
 [图表类型（报表生成器和 SSRS）](../../reporting-services/report-design/chart-types-report-builder-and-ssrs.md)   
 [条形图（报表生成器和 SSRS）](../../reporting-services/report-design/bar-charts-report-builder-and-ssrs.md)   
 [范围图（报表生成器和 SSRS）](../../reporting-services/report-design/range-charts-report-builder-and-ssrs.md)   
 [教程：向报表添加条形图（报表生成器）](../../reporting-services/tutorial-add-a-bar-chart-to-your-report-report-builder.md)   
 [图表中的空白和 Null 数据点（报表生成器和 SSRS）](../../reporting-services/report-design/empty-and-null-data-points-in-charts-report-builder-and-ssrs.md)  
  
  
