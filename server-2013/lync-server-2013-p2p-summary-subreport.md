﻿---
title: P2P 요약 하위 보고서
TOCTitle: P2P 요약 하위 보고서
ms:assetid: fc36185a-3cc5-4167-8c93-8a755fa75ac7
ms:mtpsurl: https://technet.microsoft.com/ko-kr/library/JJ205416(v=OCS.15)
ms:contentKeyID: 49305620
ms.date: 08/24/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# P2P 요약 하위 보고서

 

_**마지막으로 수정된 항목:** 2015-03-09_

P2P 요약 하위 보고서는 실패한 피어 투 피어 통신 세션에 대한 전체 보기를 제공합니다.

## 필터

필터를 사용하면 여러 방식으로 반환된 데이터를 보거나 보다 세부적으로 대상화된 데이터 집합을 반환할 수 있습니다. 다음 표에는 P2P 요약 하위 보고서에 사용할 수 있는 필터가 나와 있습니다.

### P2P 요약 하위 보고서 필터

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>이름</th>
<th>설명</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>시작</strong></p></td>
<td><p>시간 범위의 시작 날짜 및 시간입니다. 시간별 데이터를 보려면 다음과 같이 시작 날짜와 시간을 모두 입력합니다.</p>
<p>7/7/2012 1:00 PM</p>
<p>시작 시간을 입력하지 않으면 보고서가 자동으로 지정된 날짜의 오전 12시에 시작됩니다. 일별 데이터를 보려면 날짜만 입력합니다.</p>
<p>7/7/2012</p>
<p>주 또는 월별로 보려면 데이터를 보려는 해당 주 또는 월에 속하는 날짜를 입력합니다. 주 또는 월의 첫 번째 날짜를 입력할 필요가 없습니다.</p>
<p>7/3/2012</p>
<p>주는 항상 일요일부터 토요일까지입니다.</p></td>
</tr>
<tr class="even">
<td><p><strong>종료</strong></p></td>
<td><p>시간 범위의 종료 날짜 및 시간입니다. 시간별 데이터를 보려면 다음과 같이 종료 날짜 및 시간을 입력합니다.</p>
<p>7/7/2012 1:00 PM</p>
<p>종료 시간을 입력하지 않으면 보고서가 자동으로 지정된 날짜의 오전 12시에 종료됩니다. 일별 데이터를 보려면 날짜만 입력합니다.</p>
<p>7/7/2012</p>
<p>주 또는 월별로 보려면 데이터를 보려는 해당 주 또는 월에 속하는 날짜를 입력합니다. 주 또는 월의 첫 번째 날짜를 입력할 필요가 없습니다.</p>
<p>7/3/2012</p>
<p>주는 항상 일요일부터 토요일까지입니다.</p></td>
</tr>
<tr class="odd">
<td><p><strong>풀</strong></p></td>
<td><p>등록자 풀 또는 에지 서버의 FQDN(정규화된 도메인 이름)입니다. 개별 풀을 선택하거나 <strong>[모두]</strong>를 클릭하여 모든 풀에 대한 데이터를 봅니다. 이 드롭다운 목록은 데이터베이스의 레코드에 따라 자동으로 채워집니다.</p></td>
</tr>
</tbody>
</table>


## 메트릭

다음 표에는 P2P 요약 하위 보고서에 제공된 정보가 나와 있습니다.

### P2P 요약 하위 보고서 메트릭

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>이름</th>
<th>해당 항목을 기준으로 정렬 가능 여부</th>
<th>설명</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>총 세션</strong></p></td>
<td><p>아니요</p></td>
<td><p>성공한 세션, 실패한 세션(예상 오류 및 예기치 않은 오류 모두) 및 분류되지 않은 세션을 포함한 총 세션 수입니다.</p></td>
</tr>
<tr class="even">
<td><p><strong>실패율</strong></p></td>
<td><p>아니요</p></td>
<td><p>실패한 피어 투 피어 세션의 비율입니다.</p></td>
</tr>
<tr class="odd">
<td><p><strong>형식별 세션(Sessions by Modality)</strong></p></td>
<td><p>아니요</p></td>
<td><p>형식(예: 인스턴트 메시징)별로 그룹화된 총 세션 수입니다.</p></td>
</tr>
<tr class="even">
<td><p><strong>형식별 실패율(Failure rate by modality)</strong></p></td>
<td><p>아니요</p></td>
<td><p>형식(예: 인스턴트 메시징)별로 그룹화된 총 실패 세션 수입니다.</p></td>
</tr>
</tbody>
</table>

