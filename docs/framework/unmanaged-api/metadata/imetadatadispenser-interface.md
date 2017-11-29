---
title: "IMetaDataDispenser 인터페이스"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: IMetaDataDispenser
api_location: mscoree.dll
api_type: COM
f1_keywords: IMetaDataDispenser
helpviewer_keywords: IMetaDataDispenser interface [.NET Framework metadata]
ms.assetid: 989840b3-9822-4ce5-a6c5-b375d3340a7a
topic_type: apiref
caps.latest.revision: "11"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: c5a0464f2fb7b81d98fcbb4b04bc465cf57b1b0f
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2017
---
# <a name="imetadatadispenser-interface"></a><span data-ttu-id="66aac-102">IMetaDataDispenser 인터페이스</span><span class="sxs-lookup"><span data-stu-id="66aac-102">IMetaDataDispenser Interface</span></span>
<span data-ttu-id="66aac-103">새 메타 데이터 범위를 작성 하거나 기존 열 메서드를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="66aac-103">Provides methods to create a new metadata scope, or open an existing one.</span></span>  
  
## <a name="methods"></a><span data-ttu-id="66aac-104">메서드</span><span class="sxs-lookup"><span data-stu-id="66aac-104">Methods</span></span>  
  
|<span data-ttu-id="66aac-105">메서드</span><span class="sxs-lookup"><span data-stu-id="66aac-105">Method</span></span>|<span data-ttu-id="66aac-106">설명</span><span class="sxs-lookup"><span data-stu-id="66aac-106">Description</span></span>|  
|------------|-----------------|  
|[<span data-ttu-id="66aac-107">DefineScope 메서드</span><span class="sxs-lookup"><span data-stu-id="66aac-107">DefineScope Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadatadispenser-definescope-method.md)|<span data-ttu-id="66aac-108">새 메타 데이터를 만들 수 있는 메모리에 새 영역을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="66aac-108">Creates a new area in memory where you can create new metadata.</span></span>|  
|[<span data-ttu-id="66aac-109">OpenScope 메서드</span><span class="sxs-lookup"><span data-stu-id="66aac-109">OpenScope Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadatadispenser-openscope-method.md)|<span data-ttu-id="66aac-110">기존, 디스크에 파일을 열고 해당 메타 데이터를 메모리에 매핑합니다.</span><span class="sxs-lookup"><span data-stu-id="66aac-110">Opens an existing, on-disk file and maps its metadata into memory.</span></span>|  
|[<span data-ttu-id="66aac-111">OpenScopeOnMemory 메서드</span><span class="sxs-lookup"><span data-stu-id="66aac-111">OpenScopeOnMemory Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadatadispenser-openscopeonmemory-method.md)|<span data-ttu-id="66aac-112">기존 메타 데이터가 포함 된 메모리 영역을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="66aac-112">Opens an area of memory that contains existing metadata.</span></span> <span data-ttu-id="66aac-113">즉,이 메서드는 메타 데이터로 기존 데이터를 처리 하는 메모리의 지정된 된 영역을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="66aac-113">That is, this method opens a specified area of memory in which the existing data is treated as metadata.</span></span>|  
  
## <a name="requirements"></a><span data-ttu-id="66aac-114">요구 사항</span><span class="sxs-lookup"><span data-stu-id="66aac-114">Requirements</span></span>  
 <span data-ttu-id="66aac-115">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="66aac-115">**Platform:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="66aac-116">**헤더:** Cor.h</span><span class="sxs-lookup"><span data-stu-id="66aac-116">**Header:** Cor.h</span></span>  
  
 <span data-ttu-id="66aac-117">**라이브러리:** MsCorEE.dll에서 리소스로 사용</span><span class="sxs-lookup"><span data-stu-id="66aac-117">**Library:** Used as a resource in MsCorEE.dll</span></span>  
  
 <span data-ttu-id="66aac-118">**.NET framework 버전:**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="66aac-118">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="66aac-119">참고 항목</span><span class="sxs-lookup"><span data-stu-id="66aac-119">See Also</span></span>  
 [<span data-ttu-id="66aac-120">IMetaDataDispenserEx 인터페이스</span><span class="sxs-lookup"><span data-stu-id="66aac-120">IMetaDataDispenserEx Interface</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadatadispenserex-interface.md)  
 [<span data-ttu-id="66aac-121">메타 데이터 인터페이스</span><span class="sxs-lookup"><span data-stu-id="66aac-121">Metadata Interfaces</span></span>](../../../../docs/framework/unmanaged-api/metadata/metadata-interfaces.md)