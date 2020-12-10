---
title: json参数格式不对引发的异常
date: 2020-12-10 22:38:35
tags: java,springmvc
categories: 错误集
cover: 

---

**问题:**

```java
Caused by: com.fasterxml.jackson.core.JsonParseException: Unexpected character (' ' (code 160)): was
```

类似于这种错误都是传递参数格式不对,jackson无法正常解析json->object报出的错误.

重新检索数据格式就可以解决该类问题!