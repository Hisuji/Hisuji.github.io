---
title:  "Adapter Pattern(어댑터 패턴)"
excerpt: "클래스의 인터페이스를 사용자가 기대하는 다른 인터페이스로 변환하는 패턴"

categories:
  - DesignPattern
tags: JAVA
sidebar:
  nav: "docs"

permalink: /posts/designpattern/
---

‘[자바 디자인 패턴의 이해 - Gof Design](https://www.inflearn.com/course/%EC%9E%90%EB%B0%94-%EB%94%94%EC%9E%90%EC%9D%B8-%ED%8C%A8%ED%84%B4#)’ 인프런 강의를 수강하며 공부한 내용을 정리하였습니다.

***

1. 어댑터 패턴 정의[^definition]

  - 클래스의 인터페이스를 사용자가 기대하는 다른 인터페이스로 변환하는 패턴  
  - 장점: 호환성이 없는 인터페이스 때문에 함께 동작할 수 없는 클래스들이 함께 작동하도록 해준다.

[^definition]: 위키백과 - 어댑터 패턴
***

＊ 실습 - Adapter를 이용해 미리 구현된 기능을 요구사항에 맞춰서 변경할 수 있다.

[요구사항]

1. 두 수에 대한 다음 연산을 수행하는 객체 만들기
  - 수의 두 배의 수를 반환 : twiceOf(Float)
  - 수의 1/2의 수를 반환 : halfOf(Float)

2. 구현 객체 이름은 ‘Adapter’
3. Math 클래스에서 twiceOf(Float)와 halfOf(Float)는 이미 구현

[추가 요구사항]

1. Math 클래스에 수의 두배의 수를 반환하는 doubled(Double)를 추가하고 이를 이용해 프로그램을 수정

[UML - 클래스다이어그램]

<img src="https://user-images.githubusercontent.com/47530310/66184361-c7152980-e6b6-11e9-9e25-a1639c54be15.PNG" alt="디자인 패턴 클래스다이어그램" width="70%">

[실습 소스코드]

[Github](https://github.com/Hisuji/DesignPattern/tree/master/src/strategy)