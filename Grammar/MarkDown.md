<h1 id = "top">Markdown</h1>
===

<br>
<br>

What is Markdown
---
<br>

마크다운은 마크업언어의 일종이다.
마크다운문법은 읽기도 쉽고 쓰기도 쉽다는 장점이 있다.
확장자는 .md를 사용한다.

<br>
<br>

Paragraph
---
<br>

문장의 집합을 문단이라고 한다. 한 문단과 다음 문단 사이는 빈 줄로 구분된다.

<br>
<br>

Block quote
---
<br>

\>를 사용하면
>이렇게 된다


\>>를 사용하면
>>이렇게 된다.

<br>
<br>

Code
---
<br>

\```백틱을 사용하여 코드블럭을 표현할 수 있다.

예시

 >\```java (표현 언어) <br>
System.out.println("HelloWorld"); <br>
 \```

```java
System.out.println("HelloWorld");
```

Emphasis
---

<br>
<br>

italic : ** *italic*

bold : **** **bold**

line : <br><br>
\*\*\*<br>
***
\-\-\-

--- 

<br>
<br>

List
---

<br>

\-를 사용해서 구분가능 계층 구분을 위해서는 Tab을 입력해주자.

  - 1
    - 2
      - 3
        - 4
          - 5 

<br>
<br>

Link
---

<br>

```
[링크이름](https://github.com/beomsookim96)
```
[링크이름](https://github.com/beomsookim96)

<br>

```

[다른문서로]\[1]가볼까?
```
```
[1]: Thymeleaf.md "타임리프" 
```
[1]: Thymeleaf.md "타임리프"

<br>

[다른문서로][1]돌아가볼까?


<br>


```
<https://github.com/beomsookim96>
``` 

<https://github.com/beomsookim96>

<br>

```
[맨위로 돌아가자](#top)<br>
```
[맨위로 돌아가자](#top)

<br>
<br>

Table
---

```
| Header One | Header Two | Header Three | Header Four |
| ---------- | :--------- | :----------: | ----------: |
| Default    | Left       | Center       | Right       |
```
| Header One | Header Two | Header Three | Header Four |
| ---------- | :--------- | :----------: | ----------: |
| Default    | Left       | Center       | Right       |

```
| Column 1 | Column 2 | Column 3 | Column 4 |
| -------- | :------: | -------- | :--------: |
| No span  | Span across two columns||   hi   |
```
| Column 1 | Column 2 | Column 3 | Column 4 |
| -------- | :------: | -------- | :--------: |
| No span  | Span across two columns||   hi   |

<br>
<br>
<br>
[참조글](https://eungbean.github.io/2018/06/11/How-to-use-markdown/)
