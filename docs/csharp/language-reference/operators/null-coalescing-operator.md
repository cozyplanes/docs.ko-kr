---
title: ?? 연산자(C# 참조)
ms.date: 07/20/2015
f1_keywords:
- ??_CSharpKeyword
helpviewer_keywords:
- coalesce operator [C#]
- ?? operator [C#]
- conditional-AND operator (&&) [C#]
ms.assetid: 088b1f0d-c1af-4fe1-b4b8-196fd5ea9132
ms.openlocfilehash: 03d81d4216dabce2ea75b9fdcf6ef0971cc32490
ms.sourcegitcommit: 2eceb05f1a5bb261291a1f6a91c5153727ac1c19
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/04/2018
ms.locfileid: "43530108"
---
# <a name="-operator-c-reference"></a>?? 연산자(C# 참조)
`??` 연산자는 null 병합 연산자라고 합니다.  이 연산자는 피연산자가 null이 아닐 경우 왼쪽 피연산자를 반환하고 null일 경우 오른쪽 피연산자를 반환합니다.  
  
## <a name="remarks"></a>설명  
 nullable 형식은 형식 도메인의 값을 나타낼 수 있거나 값을 정의하지 않을 수 있습니다(이 경우 값은 null). 왼쪽 연산자에 값이 null인 null 허용 형식이 있는 경우 `??` 연산자의 구문 표현을 사용하여 적절한 값을 반환할 수 있습니다(오른쪽 피연산자). `??` 연산자를 사용하지 않고 nullable 값 형식을 nullable이 아닌 값 형식에 할당하려고 하면 컴파일 타임 오류가 발생합니다. 캐스트를 사용할 때 nullable 값 형식이 현재 정의되어 있지 않으면 `InvalidOperationException` 예외가 throw됩니다.  
  
 자세한 내용은 [Null 허용 형식](../../../csharp/programming-guide/nullable-types/index.md)을 참조하세요.  
  
 ?? 연산자의 결과는 해당 두 인수가 모두 상수인 경우에도 상수로 간주되지 않습니다.  
  
## <a name="example"></a>예  
 [!code-csharp[csRefOperators#53](../../../csharp/language-reference/operators/codesnippet/CSharp/null-conditional-operator_1.cs)]  
  
## <a name="see-also"></a>참고 항목

- [C# 참조](../../../csharp/language-reference/index.md)  
- [C# 프로그래밍 가이드](../../../csharp/programming-guide/index.md)  
- [C# 연산자](../../../csharp/language-reference/operators/index.md)  
- [Nullable 형식](../../../csharp/programming-guide/nullable-types/index.md)  
- [What Exactly Does ‘Lifted’ mean?](https://blogs.msdn.microsoft.com/ericlippert/2007/06/27/what-exactly-does-lifted-mean/)(‘리프트’란 정확히 어떤 의미인가요?)
