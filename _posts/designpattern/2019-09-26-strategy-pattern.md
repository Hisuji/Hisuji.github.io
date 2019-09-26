---
title:  "Strategy Pattern(스트래티지 패턴)"
excerpt: "여러 알고리즘을 하나의 추상적인 접근점을 만들어 접근점에서 서로 교환 가능하도록 하는 패턴"

categories:
  - DesignPattern
tags: JAVA
sidebar:
  nav: "docs"

permalink: /posts/designpattern/
---

‘[자바 디자인 패턴의 이해 - Gof Design](https://www.inflearn.com/course/%EC%9E%90%EB%B0%94-%EB%94%94%EC%9E%90%EC%9D%B8-%ED%8C%A8%ED%84%B4#)’ 인프런 강의를 수강하며 공부한 내용을 정리하였습니다.

***

1. 디자인 패턴 정의

  - 자주 사용하는 설계 형태를 정형화해서 이를 유형별로 설계 템플릿을 만들어둔 것 [^definition]
  - 장점: 효율성과 재사용성을 높일 수 있다.

[^definition]: NAVER 지식백과 - 디자인 패턴의 이해
***

2. 스트래티지 패턴 정의

- 여러 알고리즘을 하나의 <u>추상적인 접근점(=인터페이스)</u>을 만들어 접근점에서 서로 교환 가능하도록 하는 패턴

  1) 인터페이스 정의

	- 기능에 대한 선언과 구현 분리, 기능을 사용하는 통로로 이용

  2) 델리게이트 정의

	- 특정 객체의 기능을 사용하기 위해 다른 객체의 기능을 호출하는 것

***

＊ 실습

[요구사항]
1. 게임 캐릭터와 무기를 구현, 무기는 활과 검 두 가지 종류

[UML - 클래스다이어그램]

<img src="https://user-images.githubusercontent.com/47530310/65669748-1340e800-e07f-11e9-81f9-b13fe4ef9bab.PNG" alt="스트래티지 패턴 클래스다이어그램" width="70%">

[실습 소스코드]

[Github](https://github.com/Hisuji/DesignPattern/tree/master/src/strategy)

