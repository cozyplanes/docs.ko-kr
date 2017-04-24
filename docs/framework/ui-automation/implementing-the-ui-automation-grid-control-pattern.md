---
title: "Implementing the UI Automation Grid Control Pattern | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-bcl"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "control patterns, grid"
  - "grid control pattern"
  - "UI Automation, grid control pattern"
ms.assetid: 234d11a0-7ce7-4309-8989-2f4720e02f78
caps.latest.revision: 27
author: "Xansky"
ms.author: "mhopkins"
manager: "markl"
caps.handback.revision: 27
---
# Implementing the UI Automation Grid Control Pattern
> [!NOTE]
>  이 설명서는 <xref:System.Windows.Automation> 네임스페이스에 정의된 관리되는 [!INCLUDE[TLA2#tla_uiautomation](../../../includes/tla2sharptla-uiautomation-md.md)] 클래스를 사용하려는 .NET Framework 개발자를 위한 것입니다.[!INCLUDE[TLA2#tla_uiautomation](../../../includes/tla2sharptla-uiautomation-md.md)]에 대한 최신 정보는 [Windows 자동화 API: UI 자동화](http://go.microsoft.com/fwlink/?LinkID=156746)를 참조하세요.  
  
 이 항목에서는 속성, 메서드 및 이벤트에 대한 정보를 포함하여 <xref:System.Windows.Automation.Provider.IGridProvider>를 구현하기 위한 지침 및 규칙을 제공합니다. 추가 참조에 대한 링크는 개요의 끝에 나열되어 있습니다.  
  
 <xref:System.Windows.Automation.GridPattern> 컨트롤 패턴은 자식 요소 컬렉션에 컨테이너 역할을 하는 컨트롤을 지원하는 데 사용됩니다. 이 요소의 자식 항목은 <xref:System.Windows.Automation.Provider.IGridItemProvider>를 구현해야 하며 행과 열로 트래버스할 수 있는 2차원의 논리적 좌표계로 구성되어야 합니다. 이 컨트롤 패턴을 구현하는 컨트롤의 예제를 보려면 [Control Pattern Mapping for UI Automation Clients](../../../docs/framework/ui-automation/control-pattern-mapping-for-ui-automation-clients.md)을 참조하세요.  
  
<a name="Implementation_Guidelines_and_Conventions"></a>   
## 구현 지침 및 규칙  
 Grid 컨트롤 패턴을 구현할 때는 다음 지침 및 규칙에 유의하세요.  
  
-   Grid 좌표는 0부터 시작하며, 로캘에 따라 왼쪽 상단 또는 오른쪽 상단 셀의 좌표가 \(0, 0\)입니다.  
  
-   셀이 비어 있더라도 UI 자동화 요소가 반환되어야 해당 셀의 <xref:System.Windows.Automation.Provider.IGridItemProvider.ContainingGrid%2A> 속성을 지원할 수 있습니다. 이러한 상황은 표에 있는 자식 요소의 레이아웃이 비정형 배열과 비슷할 때 발생합니다.  
  
 ![보기 좋지 않은 레이아웃의 Windows 탐색기 보기](../../../docs/framework/ui-automation/media/uia-gridpattern-ragged-array.PNG "UIA\_GridPattern\_Ragged\_Array")  
비어 있는 좌표에서 표 컨트롤의 예  
  
-   단일 항목이 있는 표가 논리적으로 표로 간주되는 경우 이 표는 <xref:System.Windows.Automation.Provider.IGridProvider> 구현에 필요합니다. 표에서 자식 항목의 개수는 중요하지 않습니다.  
  
-   공급자 구현에 따라 숨겨진 행 및 열은 [!INCLUDE[TLA2#tla_uiautomation](../../../includes/tla2sharptla-uiautomation-md.md)] 트리에 로드될 수 있으며, 그에 따라 <xref:System.Windows.Automation.GridPattern.GridPatternInformation.RowCount%2A> 및 <xref:System.Windows.Automation.GridPattern.GridPatternInformation.ColumnCount%2A> 속성에 반영됩니다. 숨겨진 행 및 열이 아직 로드되지 않았으면 반영되지 않습니다.  
  
-   <xref:System.Windows.Automation.Provider.IGridProvider>는 표의 활성 구현을 사용하도록 설정하지 않습니다. 이 기능을 사용하려면 <xref:System.Windows.Automation.Provider.ITransformProvider>를 구현해야 합니다.  
  
-   추가, 제거 또는 병합된 셀과 같이 표의 구조 또는 레이아웃 변경 내용을 수신하려면 <xref:System.Windows.Automation.StructureChangedEventHandler>를 사용합니다.  
  
-   표의 항목 또는 셀의 이동을 추적하려면 <xref:System.Windows.Automation.AutomationFocusChangedEventHandler>를 사용합니다.  
  
<a name="Required_Members_for_IGridProvider"></a>   
## IGridProvider에 필요한 멤버  
 IGridProvider 인터페이스를 구현하려면 다음과 같은 속성 및 메서드가 필요합니다.  
  
|필요한 멤버|형식|노트|  
|------------|--------|--------|  
|<xref:System.Windows.Automation.Provider.IGridProvider.RowCount%2A>|속성|없음|  
|<xref:System.Windows.Automation.Provider.IGridProvider.ColumnCount%2A>|속성|없음|  
|<xref:System.Windows.Automation.Provider.IGridProvider.GetItem%2A>|메서드|없음|  
  
 이 컨트롤 패턴에 연결된 이벤트가 없습니다.  
  
<a name="Exceptions"></a>   
## 예외  
 공급자는 다음과 같은 예외를 throw해야 합니다.  
  
|예외 형식|조건|  
|-----------|--------|  
|<xref:System.ArgumentOutOfRangeException>|<xref:System.Windows.Automation.Provider.IGridProvider.GetItem%2A><br /><br /> -   요청된 행 좌표가 <xref:System.Windows.Automation.Provider.IGridProvider.RowCount%2A>보다 크거나 열 좌표가 <xref:System.Windows.Automation.Provider.IGridProvider.ColumnCount%2A>보다 큰 경우.|  
|<xref:System.ArgumentOutOfRangeException>|<xref:System.Windows.Automation.Provider.IGridProvider.GetItem%2A><br /><br /> -   요청된 행 또는 열의 좌표가 0보다 작은 경우.|  
  
## 참고 항목  
 [UI Automation Control Patterns Overview](../../../docs/framework/ui-automation/ui-automation-control-patterns-overview.md)   
 [Support Control Patterns in a UI Automation Provider](../../../docs/framework/ui-automation/support-control-patterns-in-a-ui-automation-provider.md)   
 [UI Automation Control Patterns for Clients](../../../docs/framework/ui-automation/ui-automation-control-patterns-for-clients.md)   
 [Implementing the UI Automation GridItem Control Pattern](../../../docs/framework/ui-automation/implementing-the-ui-automation-griditem-control-pattern.md)   
 [UI Automation Tree Overview](../../../docs/framework/ui-automation/ui-automation-tree-overview.md)   
 [Use Caching in UI Automation](../../../docs/framework/ui-automation/use-caching-in-ui-automation.md)