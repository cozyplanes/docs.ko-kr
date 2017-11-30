---
title: "ICorProfilerCallback5::ConditionalWeakTableElementReferences 메서드"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorProfilerCallback5.ConditionalWeakTableReferences
api_location: Mscorwks.dll
api_type: COM
f1_keywords: CondiitonalWeakTableElementReferences
helpviewer_keywords:
- ConditionalWeakTableElementReferences method, ICorProfilerCallback5 interface [.NET Framework profiling]
- ICorProfilerCallback5::ConditionalWeakTableElementReferences method [.NET Framework profiling]
ms.assetid: 532c7a02-a9de-4cea-bb2b-7f470da594de
topic_type: apiref
caps.latest.revision: "7"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: 386cbffea565e6864a77132b96756c073e33fc6d
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/18/2017
---
# <a name="icorprofilercallback5conditionalweaktableelementreferences-method"></a>ICorProfilerCallback5::ConditionalWeakTableElementReferences 메서드
직접 멤버 필드 참조와 `ConditionalWeakTable` 종속성을 모두 사용하여 루트를 통해 참조되는 개체의 전이적 Closure를 식별합니다.  
  
## <a name="syntax"></a>구문  
  
```  
HRESULT ConditionalWeakTableElementReferences(     [in]                     ULONG    cRootRefs,     [in, size_is(cRootRefs)] ObjectID keyRefIds[],     [in, size_is(cRootRefs)] ObjectID valueRefIds[],     [in, size_is(cRootRefs)] GCHandleID rootIds[]);};  
```  
  
#### <a name="parameters"></a>매개 변수  
 `cRootRefs`  
 [in] `keyRefIds`, `valueRefIds` 및 `rootIds` 배열의 요소 수입니다.  
  
 `keyRefIds`  
 [in] 각각 종속 핸들 쌍의 주 요소에 대한 `ObjectID`를 포함하는 개체 ID의 배열입니다.  
  
 `valueRefIds`  
 [in] 각각 종속 핸들 쌍의 보조 요소에 대한 `ObjectID`를 포함하는 개체 ID의 배열입니다. (`keyRefIds[i]` 유지 `valueRefIds[i]` 연결 유지 합니다.)  
  
 `rootIds`  
 [in] 가비지 수집 루트에 대한 추가 정보를 포함하는 정수를 가리키는 `GCHandleID` 값의 배열입니다.  
  
 콜백 자체가 진행되는 동안 `ObjectID` 메서드에서 반환되는 `ConditionalWeakTableElementReferences` 값은 유효하지 않습니다. 가비지 수집기가 이전 위치에서 새 위치로 개체를 이동하는 중일 수 있기 때문입니다. 그러므로 프로파일러는 `ConditionalWeakTableElementReferences` 호출 중에 개체 검사를 시도하지 않아야 합니다. `GarbageCollectionFinished` 시에는 모든 개체가 새 위치로 이동했으므로 검사를 수행해도 됩니다.  
  
## <a name="example"></a>예제  
 다음 코드 예제에서는 구현 하는 방법을 보여 줍니다. [ICorProfilerCallback5](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback5-interface.md) 이 방법을 사용 하 여 합니다.  
  
```  
HRESULT Callback5Impl::ConditionalWeakTableElementReferences(  
    ULONG      cRootRefs,  
    ObjectID   keyRefIds[],  
    ObjectID   valueRefIds[],  
    GCHandleID rootIds[])  
{  
    printf("Callback5Impl::ConditionalWeakTableElementReferences called\n");  
    for (unsigned int i = 0; i < cRootRefs; ++i)  
    {  
        // Save dependency to XML for later retrieval  
        PersistDependencyToXml(rootIds[i], keyRefIds[i], valueRefIds[i]);  
        // or store dependency to an internal map  
        m_cwt_deps->add_dep(rootIds[i], keyRefIds[i], valueRefIds[i]);  
        // or add arc to object graph  
        m_obj_graph->add_arc(keyRefIds[i], valueRefIds[i], rootIds[i]);  
    }  
    return S_OK;  
}  
```  
  
## <a name="remarks"></a>설명  
 에 대 한 프로파일러는 [!INCLUDE[net_v45](../../../../includes/net-v45-md.md)] 또는 이후 버전 구현 하는 [ICorProfilerCallback5](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback5-interface.md) 인터페이스 및 지정 하는 종속성 레코드는 `ConditionalWeakTableElementReferences` 메서드. `ICorProfilerCallback5`으로 표시 하는 라이브 개체 간의 종속성의 전체 집합을 제공 `ConditionalWeakTable` 항목입니다. 이러한 종속성과 멤버 필드에서 지정 된 참조는 [icorprofilercallback:: Objectreferences](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback-objectreferences-method.md) 메서드 라이브 개체의 전체 개체 그래프를 생성 하는 관리 되는 프로파일러를 사용할 수 있습니다.  
  
## <a name="requirements"></a>요구 사항  
 **플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.  
  
 **헤더:** CorProf.idl, CorProf.h  
  
 **.NET framework 버전:**[!INCLUDE[net_current_v45plus](../../../../includes/net-current-v45plus-md.md)]  
  
## <a name="see-also"></a>참고 항목  
 [ICorProfilerCallback5 인터페이스](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback5-interface.md)