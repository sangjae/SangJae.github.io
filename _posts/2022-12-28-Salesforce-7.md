---
permalink: /diary/
title: "Salesforce 오늘의 지식"
toc: true
toc_sticky: true
toc_label: "MYSELF"
---

# **Salesforce 오늘의 지식**

Validation Rule 에서 정규식 사용

한글 제한 (영문, 숫자, ",", "-", "_" 만 허용.) 하고 싶을 때,

`NOT(REGEX(필드명 ,"[a-zA-Z0-9\\.\\_\\-]*"))`

한글만 허용 하고 싶을 때,

`NOT(REGEX(필드명 ,"'ㄱ-ㅎ가-힣'*"))`