---
permalink: /diary/
title: "Salesforce 오늘의 지식"
toc: true
toc_sticky: true
toc_label: "MYSELF"
---

# **Salesforce 오늘의 지식**
Chatter를 Apex에서 사용하면서, Record를 링크걸고 싶을 때,
Chatter 관련 Apex에서 호출해서 넣을 때, 설정할 것.

SetUp > Feature Settings > Feed Tracking 메뉴에서

Link걸 Object를 선택하고 Enable Feed Tracking을 활성화 시켜주어야 Chatter Feed에서 사용할 수 있다.


주의사항 : 
다른 필드를 모두 입력할 필요는 없다. 해당 기능은 Object의 변동사항을 Tracking할 목적으로 알림을 받는 것인데, 해당 용도로 사용할 것이 아니라면, 활성화만으로도 Apex에서 Feed를 보낼 수 있다.