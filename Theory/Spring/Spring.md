###JPA, Hibernate, Repository // Comparison

<a href="https://whitekeyboard.tistory.com/264?category=819697">참고자료</a>

JPA는 라이브러리가 아닌 인터페이스이다.<br>
Hibernate는 JPA를 사용하기 위한 구현체이다. 반드시 Hibernate를 사용할 필요는 없다.<br>
Repository 는 Spring Data JPA의 핵심. JPA를 한 단계 추상화시킨 Repository라는 인터페이스를 제공한다.
<br>Repository 인터페이스에 정해진 규칙대로 메소드를 입력하면 메소드 이름에 따라 쿼리를 던지는 구현체를 Bean으로 등록한다.
