---
title: "자바 배워보기-메소드"
date: "2022-02-08 1:22:30 +0200"
author: 김지훈
category: java
---

자바의 메소드에 대해 배워보자.


메소드
===
***
프로그래밍을 하다보면 같은 코드를 여러번 쓸 때가 있고, 코드 압축을 위해 함수를 쓰는 경우가 있다.

하지만 자바는 객체지향 언어이기 때문에 함수가 존재하지 않는다.

그 대신 자바에선 함수와 비슷한 메소드를 쓴다.

예시
---
***
```java
public class Test{
    int sum (int a,int b){
        return a+b;
    }

    public static void main(String[] args){

        int i = sum(3,4);
        System.out.print(i);
        
    }
}
```
위의 코드는 ```sum```이라는 이름의 메소드에 3 과 4를 입력해 ```sum```의 값을 출력하는 코드이다.


메소드는 값을 입력받고 메소드 안의 명령문을 실행하고 값을 출력하며, 우리가 흔히 아는 함수와 작동 방식이 같다.

그러나 메소드는 입력을 받지 않을수도 있고, 리턴을 하지 않을수도 있기에 입력이 없거나, 리턴값이 없거나, 혹은 둘다 없을 수도 있다.

위의 메소드는 입력값과 리턴이 둘아 있는 경우다.

### 입력이 없는 메소드
***
```java
String testMethod(){
    return "thisistest"
}
```

위같은 경우는 입력이 없고, 리턴값인 "thisistest"만 출력하는 메소드이다.

출력할 자료형을 String으로 해놨으므로 "thisistest"의 자료형은 String이다.
### 리턴이 없는 메소드
***
```java
void printSum(int a,int b){
    System.out.printf(a+b);
}
```
위같은 경우는 리턴값이 없고, a와 b를 받아 그 합을 출력하기만 하는 메소드이다.

### 입력과 리턴이 없는 메소드
***
```java
int printStr(){
    System.out.printf("helloworld");
}
```
```java
위같은 경우는 입력값과 리턴값이 둘 다 없고, "helloworld"만 출력하는 메소드이다.

return 응용하기
---
***
return은 메소드를 실행한 뒤 값을 반환하는 기능도 있지만, 실행하는 즉시 메소드가 종료되기 때문에 여러 방법으로 응용할수 있다.