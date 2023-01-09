---
permalink: /diary/
title: "Salesforce 오늘의 지식"
toc: true
toc_sticky: true
toc_label: "MYSELF"
---

# **Salesforce 오늘의 지식**

모바일 CSS 분기 처리 하는 방법 .js에서

```
// Device Type 별 css Class 추가를 위한 변수 설정

    if($A.get("$Browser.formFactor") == 'DESKTOP'){

      deviceType = 'isDesktop';

    } else if ($A.get("$Browser.formFactor") == 'PHONE') {

      if($A.get("$Browser.isIOS")){

        deviceType = 'isIOS';

      } else if($A.get("$Browser.isAndroid")){

        deviceType = 'isAndroid';

      } else if($A.get("$Browser.isTablet")){

        deviceType = 'isTablet';

      } else if($A.get("$Browser.isWindowsPhone")){

        deviceType = 'isWindowsPhone';

      } else {

        deviceType = 'isPHONE';

      }

    } else {

      deviceType = 'isOther';

    }



    component.set('v.deviceType', deviceType);

**************cmp



<div class="{! 'slds-form-element_horizontal ' + v.deviceType}">
```
