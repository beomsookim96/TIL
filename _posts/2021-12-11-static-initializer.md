---
layout: post
title: static-intializer
description: static-intializer
tags: java
minute: 1
---

#### Static initializer block

```java

private int a;
private int b;
private boolean flag;

static{

    a = 1;
    b = 2;

    if(a*b > 0){

        flag = true;

    }else{

        flag = false;

    }

}
```

flag기법도 함께 알아두자!