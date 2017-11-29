---
title: "ISymUnmanagedVariable::GetSignature 메서드"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ISymUnmanagedVariable.GetSignature
api_location: diasymreader.dll
api_type: COM
f1_keywords: ISymUnmanagedVariable::GetSignature
helpviewer_keywords:
- GetSignature method, ISymUnmanagedVariable interface [.NET Framework debugging]
- ISymUnmanagedVariable::GetSignature method [.NET Framework debugging]
ms.assetid: 78c1ba28-a410-4360-805c-23a95408964a
topic_type: apiref
caps.latest.revision: "8"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: 1e29cd4a38e9abbe380b51b81fc2849b833d87e9
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/18/2017
---
# <a name="isymunmanagedvariablegetsignature-method"></a><span data-ttu-id="413a3-102">ISymUnmanagedVariable::GetSignature 메서드</span><span class="sxs-lookup"><span data-stu-id="413a3-102">ISymUnmanagedVariable::GetSignature Method</span></span>
<span data-ttu-id="413a3-103">이 변수 시그니처를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="413a3-103">Gets the signature of this variable.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="413a3-104">구문</span><span class="sxs-lookup"><span data-stu-id="413a3-104">Syntax</span></span>  
  
```  
HRESULT GetSignature(  
    [in]  ULONG32  cSig,  
    [out] ULONG32  *pcSig,  
    [out, size_is(cSig),  
        length_is(*pcSig)] BYTE sig[]);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="413a3-105">매개 변수</span><span class="sxs-lookup"><span data-stu-id="413a3-105">Parameters</span></span>  
 `cSig`  
 <span data-ttu-id="413a3-106">[in] 가리키는 버퍼의 길이 `sig` 매개 변수입니다.</span><span class="sxs-lookup"><span data-stu-id="413a3-106">[in] The length of the buffer pointed to by the `sig` parameter.</span></span>  
  
 `pcSig`  
 <span data-ttu-id="413a3-107">[out] 에 대 한 포인터는 `ULONG32` 시그니처를 포함 하는 데 필요한 버퍼의 문자에는 크기를 받는 합니다.</span><span class="sxs-lookup"><span data-stu-id="413a3-107">[out] A pointer to a `ULONG32` that receives the size, in characters, of the buffer required to contain the signature.</span></span>  
  
 `sig`  
 <span data-ttu-id="413a3-108">[out] 서명을 저장 하는 버퍼입니다.</span><span class="sxs-lookup"><span data-stu-id="413a3-108">[out] The buffer that stores the signature.</span></span>  
  
## <a name="return-value"></a><span data-ttu-id="413a3-109">반환 값</span><span class="sxs-lookup"><span data-stu-id="413a3-109">Return Value</span></span>  
 <span data-ttu-id="413a3-110">메서드가 성공 하면 s_ok이 고 그렇지 않으면 E_FAIL 또는 일부 기타 오류 코드입니다.</span><span class="sxs-lookup"><span data-stu-id="413a3-110">S_OK if the method succeeds; otherwise, E_FAIL or some other error code.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="413a3-111">요구 사항</span><span class="sxs-lookup"><span data-stu-id="413a3-111">Requirements</span></span>  
 <span data-ttu-id="413a3-112">**헤더:** CorSym.idl, CorSym.h</span><span class="sxs-lookup"><span data-stu-id="413a3-112">**Header:** CorSym.idl, CorSym.h</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="413a3-113">참고 항목</span><span class="sxs-lookup"><span data-stu-id="413a3-113">See Also</span></span>  
 [<span data-ttu-id="413a3-114">ISymUnmanagedVariable 인터페이스</span><span class="sxs-lookup"><span data-stu-id="413a3-114">ISymUnmanagedVariable Interface</span></span>](../../../../docs/framework/unmanaged-api/diagnostics/isymunmanagedvariable-interface.md)