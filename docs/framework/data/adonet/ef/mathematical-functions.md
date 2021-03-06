---
title: 수학 함수
ms.date: 03/30/2017
ms.assetid: b040c7cb-156d-40f2-9152-61065b18148c
ms.openlocfilehash: e6c58d781d7138f8295f2d0a2f0db110ad4b1dd6
ms.sourcegitcommit: fb78d8abbdb87144a3872cf154930157090dd933
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/26/2018
ms.locfileid: "47203946"
---
# <a name="mathematical-functions"></a>수학 함수

.NET Framework Data Provider for SQL Server(SqlClient)에서는 인수로 제공된 입력 값에 대해 계산을 수행한 다음 숫자 값으로 된 결과를 반환하는 수치 연산 함수를 제공합니다. 이 함수는 SqlClient를 사용할 때 사용 가능한 SqlServer 네임스페이스에 있습니다. 공급자의 네임스페이스 속성이 있으면 특정 구문(예: 형식 및 함수)에 대해 이 공급자가 사용하는 접두사를 Entity Framework에서 찾을 수 있습니다. 다음 표에서는 SqlClient 수치 함수에 대해 설명합니다.  
  
## <a name="absexpression"></a>ABS(expression)

절대 값 함수를 수행합니다.

**인수**

`expression`: `Int32`, `Int64`, `Double` 또는 `Decimal`입니다.

**반환 값**

지정한 식의 절대 값입니다.

**예제**

`SqlServer.ABS(-2)`

## <a name="acosexpression"></a>ACOS(expression)

지정한 식의 아크코사인 값을 반환합니다.

**인수**

`expression`: `Double`입니다.

**반환 값**

`Double`

**예제**

`SqlServer.ACOS(.9)`

## <a name="asinexpression"></a>ASIN(expression)

지정한 식의 아크사인 값을 반환합니다.

**인수**

`expression`: `Double`입니다.

**반환 값**

`Double`

**예제**

`SqlServer.ASIN(.9)`

## <a name="atanexpression"></a>ATAN(expression)

지정한 숫자 식의 아크탄젠트 값을 반환합니다.

**인수**

`expression`: `Double`입니다.

**반환 값**

`Double`

**예제**

`SqlServer.ATAN(9)`

## <a name="atn2expression-expression"></a>ATN2(expression, expression)

탄젠트 값이 지정한 두 숫자 식 사이에 속하는 각도를 라디안으로 반환합니다.

**인수**

`expression`: `Double`입니다.

**반환 값**

`Double`

**예제**

`SqlServer.ATN2(9, 8)`
 
## <a name="ceilingexpression"></a>CEILING(expression)

지정한 식을 해당 식보다 크거나 같은 가장 작은 정수로 변환합니다.

**인수**

`expression`: `Int32`, `Int64`, `Double` 또는 `Decimal`입니다.

**반환 값**

`Int32`, `Int64`를 `Double`, 또는 `Decimal`합니다.

**예제** 

[!code-csharp[DP EntityServices Concepts#SQLSERVER_CEILING](~/samples/snippets/csharp/VS_Snippets_Data/dp entityservices concepts/cs/entitysql.cs#sqlserver_ceiling)]
[!code-sql[DP EntityServices Concepts#SQLSERVER_CEILING](~/samples/snippets/tsql/VS_Snippets_Data/dp entityservices concepts/tsql/entitysql.sql#sqlserver_ceiling)]

## <a name="cosexpression"></a>COS(expression)

라디안으로 지정된 각도의 삼각 코사인을 계산합니다. 

**인수** 

`expression`: `Double`입니다. 

**반환 값** 

`Double` 

**예제** 

`SqlServer.COS(45)`

## <a name="cotexpression"></a>COT(expression)

지정된 각도의 삼각 코탄젠트를 라디안으로 계산합니다. 

**인수** 

`expression`: `Double`입니다. 

**반환 값** 

`Double` 

**예제** 

`SqlServer.COT(60)`
  
## <a name="degreesradians"></a>DEGREES(radians)

해당 각도를 도 단위로 반환합니다. 

**인수** 

`expression`: `Int32`, `Int64`, `Double` 또는 `Decimal`입니다. 

**반환 값** 

`Int32`, `Int64`를 `Double`, 또는 `Decimal`합니다. 

**예제** 

`SqlServer.DEGREES(3.1)`

## <a name="expexpression"></a>EXP(expression)

지정한 숫자 식의 지수 값을 계산합니다. 

**인수** 

`expression`: `Double`입니다. 

**반환 값** 

`Double` 

**예제** `SqlServer.EXP(1)`

## <a name="floorexpression"></a>FLOOR(expression)

지정한 식을 해당 식보다 작거나 같은 가장 큰 정수로 변환합니다. 

**인수** 

`expression`: `Double`입니다. 

**반환 값** 

`Double` 

**예제** 

[!code-csharp[DP EntityServices Concepts#SQLSERVER_FLOOR](~/samples/snippets/csharp/VS_Snippets_Data/dp entityservices concepts/cs/entitysql.cs#sqlserver_floor)] 
[!code-sql[DP EntityServices Concepts#SQLSERVER_FLOOR](~/samples/snippets/tsql/VS_Snippets_Data/dp entityservices concepts/tsql/entitysql.sql#sqlserver_floor)]

## <a name="logexpression"></a>LOG(expression)

지정한 `float` 식의 자연 로그를 계산합니다. 

**인수** 

`expression`: `Double`입니다. 

**반환 값** 

`Double` 

**예제** 

`SqlServer.LOG(100)`

## <a name="log10expression"></a>LOG10(expression)

지정한 `Double` 식의 상용 로그를 반환합니다. 

**인수** 

`expression`: `Double`입니다. 

**반환 값** 

`Double` 

**예제** 

`SqlServer.LOG10(100)`

## <a name="pi"></a>PI)

파이의 상수 값을 `Double`로 반환합니다. 

**반환 값** 

`Double` 

**예제** 

`SqlServer.PI()`

## <a name="powernumericexpression-powerexpression"></a>POWER (numeric_expression, power_expression)

지정한 숫자 식의 지정된 거듭제곱 값을 계산합니다.

**인수** 

|  |  |
|--|--|
|`numeric_expression`| `Int32`, `Int64`를 `Double`, 또는 `Decimal`합니다.|
|`power_expression`| `Double`에 대해 계산할 거듭제곱을 나타내는 `numeric_expression`입니다.| 

**반환 값** 

지정한 `numeric_expression`에 지정한 `power_expression`을 거듭제곱한 값입니다. 

**예제** 

`SqlServer.POWER(2,7)`

## <a name="radiansexpression"></a>RADIANS(expression)

각도를 라디안으로 변환합니다. 

**인수** 

`expression`: `Int32`, `Int64`, `Double` 또는 `Decimal`입니다. 

**반환 값** 

`Int32`, `Int64`를 `Double`, 또는 `Decimal`합니다. 

**예제** 

`SqlServer.RADIANS(360.0)`

## <a name="randseed"></a>RAND([seed])

0에서 1 사이의 임의 값을 반환합니다. 

**인수** 

시드 값으로는 `Int32`합니다. 시드를 지정하지 않으면 SQL Server 데이터베이스 엔진에서 시드 값을 임의로 할당합니다. 지정된 특정 시드 값에 대해 반환되는 결과는 항상 동일합니다.

**반환 값** 

0에서 1 사이의 임의 `Double` 값입니다. 

**예제** 

`SqlServer.RAND()`
  
## <a name="roundnumericexpression-lengthfunction"></a>ROUND(numeric_expression, length[,function])

숫자 식을 지정한 길이나 전체 자릿수로 반올림하여 반환합니다. 

**인수** 

|  |  |
|--|--|
|`numeric_expression`| `Int32`, `Int64`를 `Double`, 또는 `Decimal`합니다. 
|`length`| `Int32`을 반올림할 전체 자릿수를 나타내는 `numeric_expression`입니다. `length`가 양수일 경우 `numeric_expression`은 `length`에서 지정한 소수 자릿수로 반올림됩니다. `length`가 음수일 경우 `numeric_expression`은 `length`에서 지정한 대로 소수점의 왼쪽에서 반올림됩니다.|
|`function` | 선택 사항입니다. `Int32` 수행할 연산 형식을 나타내는입니다. 함수를 생략 하거나 값이 0 (기본값) 일 때 `numeric_expression` 반올림 됩니다. 이외의 값 0을 지정 하면 `numeric_expression` 잘립니다. |

**반환 값** 

지정한 `numeric_expression`에 지정한 `power_expression`을 거듭제곱한 값입니다.

**예제** 

`SqlServer.ROUND(748.58, -3)`

## <a name="signexpression"></a>SIGN(expression) 

지정한 식의 양수(+1), 0 또는 음수(-1) 부호를 반환합니다. 

**인수** 

`expression`: `Int32`, `Int64`, `Double` 또는 `Decimal` 

**반환 값** 

`Int32`, `Int64`를 `Double`, 또는 `Decimal`합니다. 

**예제** 

`SqlServer.SIGN(-10)`

## <a name="sinexpression"></a>SIN(expression)

라디안으로 지정한 각도의 삼각 사인을 계산하여 `Double` 식을 반환합니다. 

**인수** 

`expression`: `Double`입니다. 

**반환 값** 

`Double` 

**예제** `SqlServer.SIN(20)`

## <a name="sqrtexpression"></a>SQRT(expression)

지정한 식의 제곱근을 반환합니다. 

**인수** 

`expression`: `Double`입니다. 

**반환 값** 

`Double` 

**예제** `SqlServer.SQRT(3600)`

## <a name="squareexpression"></a>SQUARE(expression)

지정한 식의 제곱을 반환합니다. 

**인수** 

`expression`: `Double`입니다. 

**반환 값** 

`Double` 

**예제** 

`SqlServer.SQUARE(25)`

## <a name="tanexpression"></a>TAN(expression)

지정한 식의 탄젠트를 계산합니다.

**인수** 

`expression`: `Double` 

**반환 값** 

`Double` 

**예제** 

`SqlServer.TAN(45.0)`
  
## <a name="see-also"></a>참고자료

SqlClient에서 지원하는 수치 함수에 대한 자세한 내용은 SqlClient 공급자 매니페스트에 지정한 SQL Server 버전의 설명서를 참조하세요.  
  
**SQL Server 2005:** [수치 연산 함수 (TRANSACT-SQL)](https://docs.microsoft.com/previous-versions/sql/sql-server-2005/ms177516(v=sql.90))  
**SQL Server 2008:** [수치 연산 함수 (TRANSACT-SQL)](https://docs.microsoft.com/previous-versions/sql/sql-server-2008/ms177516(v=sql.100))  
**SQL Server 2012 이상:** [수치 연산 함수 (TRANSACT-SQL)](/sql/t-sql/functions/mathematical-functions-transact-sql?view=sql-server-2017)   

 [Entity Framework용 SqlClient 기능](sqlclient-for-ef-functions.md)
