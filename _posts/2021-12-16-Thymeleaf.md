---
layout: post
title: Thymeleaf
description: Thymeleaf Grammar
tags: serverside-template
minute: 1
---

###Thymeleaf Grammar

https://www.thymeleaf.org/doc/tutorials/3.0/usingthymeleaf.html

Thymeleaf is a modern server-side Java template engine for both web and standalone environments, capable of processing HTML, XML, JavaScript, CSS and even plain text.
<br>
\<html xmlns:th="http://www.thymeleaf.org">

\<p th:text="#{home.welcome}">Welcome to our grocery store!\</p>
<br>
HTML5-valid
<br>
\<p data-th-text="#{home.welcome}">Welcome to our grocery store!\</p>
