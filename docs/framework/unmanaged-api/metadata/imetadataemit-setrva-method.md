---
title: "IMetaDataEmit::SetRVA 메서드"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: IMetaDataEmit.SetRVA
api_location: mscoree.dll
api_type: COM
f1_keywords: IMetaDataEmit::SetRVA
helpviewer_keywords:
- IMetaDataEmit::SetRVA method [.NET Framework metadata]
- SetRVA method [.NET Framework metadata]
ms.assetid: 4d69fb6d-ee35-4318-8224-5eea2bd16818
topic_type: apiref
caps.latest.revision: "10"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: 25f0e20e1249067dfd9162b84c07b38e9b97de15
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2017
---
# <a name="imetadataemitsetrva-method"></a><span data-ttu-id="0ad17-102">IMetaDataEmit::SetRVA 메서드</span><span class="sxs-lookup"><span data-stu-id="0ad17-102">IMetaDataEmit::SetRVA Method</span></span>
<span data-ttu-id="0ad17-103">지정 된 메서드의 상대 가상 주소를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="0ad17-103">Sets the relative virtual address of the specified method.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="0ad17-104">구문</span><span class="sxs-lookup"><span data-stu-id="0ad17-104">Syntax</span></span>  
  
```  
HRESULT SetRVA (  
    [in]  mdMethodDef  md,   
    [in]  ULONG        ulRVA   
);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="0ad17-105">매개 변수</span><span class="sxs-lookup"><span data-stu-id="0ad17-105">Parameters</span></span>  
 `md`  
 <span data-ttu-id="0ad17-106">[in] 대상 메서드 또는 메서드 구현에 대 한 토큰입니다.</span><span class="sxs-lookup"><span data-stu-id="0ad17-106">[in] The token for the target method or method implementation.</span></span>  
  
 `ulRVA`  
 <span data-ttu-id="0ad17-107">[in] 주소는 코드 또는 데이터 영역입니다.</span><span class="sxs-lookup"><span data-stu-id="0ad17-107">[in] The address of the code or data area.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="0ad17-108">요구 사항</span><span class="sxs-lookup"><span data-stu-id="0ad17-108">Requirements</span></span>  
 <span data-ttu-id="0ad17-109">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="0ad17-109">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="0ad17-110">**헤더:** Cor.h</span><span class="sxs-lookup"><span data-stu-id="0ad17-110">**Header:** Cor.h</span></span>  
  
 <span data-ttu-id="0ad17-111">**라이브러리:** MSCorEE.dll에서 리소스로 사용</span><span class="sxs-lookup"><span data-stu-id="0ad17-111">**Library:** Used as a resource in MSCorEE.dll</span></span>  
  
 <span data-ttu-id="0ad17-112">**.NET framework 버전:**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="0ad17-112">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="0ad17-113">참고 항목</span><span class="sxs-lookup"><span data-stu-id="0ad17-113">See Also</span></span>  
 [<span data-ttu-id="0ad17-114">IMetaDataEmit 인터페이스</span><span class="sxs-lookup"><span data-stu-id="0ad17-114">IMetaDataEmit Interface</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataemit-interface.md)  
 [<span data-ttu-id="0ad17-115">IMetaDataEmit2 인터페이스</span><span class="sxs-lookup"><span data-stu-id="0ad17-115">IMetaDataEmit2 Interface</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataemit2-interface.md)