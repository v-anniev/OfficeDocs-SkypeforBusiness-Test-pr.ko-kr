﻿---
title: 'Lync Server 2013: Active Directory 스키마 준비'
TOCTitle: Active Directory 스키마 준비
ms:assetid: 067726ae-fd3f-4133-a32f-26d2603ac674
ms:mtpsurl: https://technet.microsoft.com/ko-kr/library/Gg398119(v=OCS.15)
ms:contentKeyID: 49302690
ms.date: 08/10/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Lync Server 2013에서 Active Directory 스키마 준비

 

_**마지막으로 수정된 항목:** 2012-08-27_

Active Directory 도메인 서비스 준비를 시작하기 전에 Windows 메모장 등의 텍스트 편집기를 사용하여 스키마 파일을 열거나, [Lync Server 2013에서 사용하는 Active Directory 스키마 확장, 클래스 및 속성](lync-server-2013-active-directory-schema-extensions-classes-and-attributes-used-by-lync-server.md)의 내용을 참조하여 Lync Server 2013용으로 수정할 모든 Active Directory 도메인 서비스 스키마 확장을 검토할 수 있습니다. Lync Server에서는 다음과 같은 네 개의 스키마 파일을 사용합니다.

  - ExternalSchema.ldf - Microsoft Exchange Server와의 상호 운용성을 위해 사용됩니다.

  - ServerSchema.ldf - 기본 Lync Server 2013 스키마 파일입니다.

  - BackCompatSchema.ldf - 이전 릴리스 구성 요소와의 상호 운용성을 위해 사용됩니다.

  - VersionSchema.ldf - 준비된 스키마의 버전 정보에 사용됩니다.

모든 .ldf 파일은 이전 릴리스에서 마이그레이션하든, 새 설치를 수행하든 관계없이 스키마 준비 중에 설치됩니다. 이러한 스키마 파일은 위의 목록에 나와 있는 순서대로 설치되며, 설치 미디어의 \\Support\\schema 폴더에 있습니다.

Lync Server 스키마 확장은 모든 도메인으로 복제되므로 네트워크 트래픽에 영향을 줍니다. 따라서 스키마 준비는 네트워크 사용량이 적을 때 실행해야 합니다.


> [!NOTE]
> Java용 Microsoft® Office Communicator Mobile 2007 R2 및 Nokia 1.0 모바일 클라이언트용 Microsoft® Office Communicator Mobile에 대한 지원을 Lync Server 2013 배포에 추가해야 하는 경우에는 Lync Server 2013 설치 중에 Microsoft Office Communications Server 2007 R2용 Active Directory 스키마를 준비해야 합니다. 필요한 소프트웨어 및 설명서는 <A class=uri href="http://go.microsoft.com/fwlink/?linkid=207172%26clcid=0x412">http://go.microsoft.com/fwlink/?linkid=207172&amp;clcid=0x412</A>를 참조하십시오.



## ADSI 편집

ADSI 편집(Active Directory 서비스 인터페이스 편집기)은 스키마 준비 및 복제를 확인하는 데 사용할 수 있는 AD DS 관리 도구입니다.

서버를 도메인 컨트롤러로 만들기 위해 AD DS 역할을 설치할 때 ADSI 편집이 기본적으로 설치됩니다. Windows Server 2008 및 Windows Server 2008 R2의 경우 ADSI 편집(adsiedit.msc)은 RSAT(원격 서버 관리 도구)에 포함되어 있습니다. RSAT를 도메인 구성원 서버 또는 독립 실행형 서버에 설치할 수도 있습니다. RSAT 패키지는 Windows를 설치할 때 이러한 서버에 기본적으로 복사되지만, 기본적으로 설치되지는 않습니다. 서버 관리자를 사용하여 개별 도구를 설치합니다. ADSI 편집은 **역할 관리 도구** , **Active Directory 도메인 서비스 도구** 및 **Active Directory 도메인 컨트롤러 도구** 에 포함되어 있습니다.

Windows Server 2003의 경우 ADSI 편집은 지원 도구에 포함되어 있습니다. 지원 도구는 Windows Server 2003 CD의 \\SUPPORT\\TOOLS 폴더에 있으며, "Windows Server 2003 서비스 팩 2 32비트 지원 도구"( [http://go.microsoft.com/fwlink/?linkid=125770\&clcid=0x412](http://go.microsoft.com/fwlink/?linkid=125770%26clcid=0x412))에서도 다운로드할 수 있습니다. 제품 CD에서 지원 도구를 설치하는 지침은 "Windows 지원 도구 설치"( [http://go.microsoft.com/fwlink/?linkid=125771\&clcid=0x412](http://go.microsoft.com/fwlink/?linkid=125771%26clcid=0x412))에서 제공됩니다. Adsiedit.dll은 지원 도구를 설치할 때 자동으로 등록됩니다. 그러나 이 파일을 컴퓨터에 그냥 복사한 경우에는 도구를 실행하기 전에 **regsvr32** 명령을 실행하여 adsiedit.dll 파일을 등록해야 합니다.

## 이 섹션의 내용

  - [Lync Server 2013에서 Active Directory 스키마 준비 실행](lync-server-2013-running-schema-preparation.md)

  - [Lync Server 2013에서 Active Directory 스키마 복제 확인](lync-server-2013-verifying-schema-replication.md)

## 참고 항목

#### 기타 리소스

[Lync Server 2013에 대한 포리스트 준비](lync-server-2013-preparing-the-forest.md)  
[Lync Server 2013에 대한 도메인 준비](lync-server-2013-preparing-domains.md)

