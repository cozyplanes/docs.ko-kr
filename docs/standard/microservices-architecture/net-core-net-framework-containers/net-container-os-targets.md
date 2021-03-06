---
title: .NET 컨테이너에서 대상으로 지정할 OS
description: 컨테이너화된 .NET 응용 프로그램을 위한 .NET 마이크로 서비스 아키텍처 | .NET 컨테이너에서 대상으로 지정할 OS
author: CESARDELATORRE
ms.author: wiwagn
ms.date: 10/18/2017
ms.openlocfilehash: fca5cf280d5abb85da78413a6eed463a2ffe6a88
ms.sourcegitcommit: 979597cd8055534b63d2c6ee8322938a27d0c87b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/29/2018
ms.locfileid: "37104881"
---
# <a name="what-os-to-target-with-net-containers"></a>.NET 컨테이너에서 대상으로 지정할 OS

Docker에서 지원하는 운영 체제의 다양함과 .NET Framework 및 .NET Core 간 차이를 고려해 보면 사용하는 프레임워크에 따라 특정 OS와 특정 버전을 목표로 해야 합니다. 

Windows의 경우 Windows Server Core 또는 Windows Nano Server를 사용할 수 있습니다. 이러한 Windows 버전은 각각 .NET Framework나 .NET Core에서 필요할 수 있는 다양한 특성(Windows Server Core의 IIS와 Nano Server의 Kestrel 같은 자체 호스팅 웹 서버)을 제공합니다. 

Linux의 경우 공식 .NET Docker 이미지(예: Debian)에서 여러 배포판을 제공합니다.

그림 3-1에서는 사용하는 .NET 프레임워크에 따라 가능한 OS 버전을 확인할 수 있습니다. 

![](./media/image1.png)

**그림 3-1.** .NET framework의 버전에 따라 대상으로 하는 운영 체제

다른 Linux 배포판을 사용하려 하거나 Microsoft에서 제공하지 않는 버전 이미지가 필요한 경우 자체 Docker 이미지를 만들 수도 있습니다. 예를 들어 .NET Framework 및Windows Server Core에서 실행되는 기존 ASP.NET Core를 통해 이미지를 만들 수 있으나 Docker에는 그렇게 일반적인 시나리오가 아닙니다.

Dockerfile 파일에 이미지 이름을 추가할 때는 다음 예제에서처럼 사용하는 태그에 따라 운영 체제와 버전을 선택할 수 있습니다.

-   microsoft/**dotnet:2.1-runtime**

        .NET Core 2.1 multi-architecture: Supports Linux and Windows Nano Server depending on the Docker host.

-   microsoft/**dotnet:2.1-aspnetcore-runtime**
    
        ASP.NET Core 2.1 multi-architecture: Supports Linux and Windows Nano Server depending on the Docker host.
        The aspnetcore image has a few optimizations for ASP.NET Core. 

-   microsoft/**dotnet:2.1-aspnetcore-runtime-alpine** 

        .NET Core 2.1 runtime-only on Linux Alpine distro

-   microsoft/**dotnet:2.1-aspnetcore-runtime-nanoserver-1803** 

        .NET Core 2.1 runtime-only on Windows Nano Server (Windows Server version 1803)




>[!div class="step-by-step"]
[이전](container-framework-choice-factors.md)
[다음](official-net-docker-images.md)
