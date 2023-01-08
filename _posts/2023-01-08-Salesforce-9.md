---
permalink: /diary/
title: "Salesforce 오늘의 지식"
toc: true
toc_sticky: true
toc_label: "MYSELF"
---

# **Salesforce 오늘의 지식**

RecordEditForm에서 submit까지 성공 후 다시 같은 화면에 들어왔을 때, 이전값을 유지하는 현상

오브젝트의 New, Edit 버튼을 Override 하여 사용할 때

RecordEditForm을 사용해서 개발해 두었을 때,

OnSuccess 이벤트에 navigate를 사용하여 이동 시키곤 했는데,

저장 후 다시 같은 페이지로 들어오면,

이전 값을 그대로 유지하고 있는 경우가 있다.



그럴때는

$A.get('e.force:refreshView').fire();

를 success 이벤트 끝에 추가하여 준다.


주의사항 : 
필드들을 reset하여 사용하면, 스크롤 위치등은 그대로 남아있게 되어 보기가 좋지 않음으로 refresh를 추천함.