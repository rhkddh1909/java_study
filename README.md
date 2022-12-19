# 자바의 소개

## 프로그램 개발 순서

1. 소스파일 생성
2. 소스파일 컴파일
3. 컴파일로 실행파일 생성
4. 컴퓨터로 실행

- 소스파일은 인간중심으로 표현된 언어(컴퓨터 인식못함) 컴파일을 통해 1과0인 기계어로 변환

## 자바 실행 파일

1. 소스파일 ->(컴파일)-> 실행파일(.class 파일, 바이트코드) ->(실행)-> JVM(바이트코드를 기계어로 변환) ->(기계어코드)-> 컴퓨터

## JVM 개요

1. class loader(프로그램을 실행가기 위해 필요한 모든 파일을 찾아 메모리에 로딩)
2. byte code vrifier(준비된 코드들의 유효성 검증)
3. interpreter | jit(just in time) compiler (바이트코드를 기계어 코드로 변환 : interpreter 명령문 단위, JIT compiler(전체 단위))
4. runtime

## ORACLE에서 설치

- JDK(JVM + 개발 TOOL) -> 개발
- JRE(JVM + etc(api 등등)) -> 단순 실행

## JAVA_HOME 설정(개발자는 JDK를 JAVA_HOME으로 설정)

- 내PC 마우스 오른쪽 → 속성 → 고급시스템설정 → 환경변수 → 새로만들기 → JAVA_HOME, JDK 폴더 PATH

## PAHT 설정

- PATH 더블 클릭 -> 새로만들기 -> %JAVA_HOME%\bin -> 확인

# 데이터 활용

## 변수 기본

- 변수 선언 : 메모리에 데이터를 저장하기 위해 일정한 공간을 확보하고 이름을 지정

## 데이터 종류

- 기본 타입
1) 논리 타입 : true or false로 두가지 값 중에 하나의 값만 저장(boolean) - 1byte
2) 문자 타입 : 한 글자의 값만 가지는 데이터를 표현(char) -> 2byte
3) 정수 타입 :

- 노션 확인 : https://www.notion.so/JAVA-1696f11d262347e48e2ece3c06ca34dd#98b546f8c96347ba81ccb57b5c99a7f1

4) 실수 타입 :

- 노션 확인 : https://www.notion.so/JAVA-1696f11d262347e48e2ece3c06ca34dd#98b546f8c96347ba81ccb57b5c99a7f1

5) 참조 타입 :

- 노션 확인 : https://www.notion.so/JAVA-1696f11d262347e48e2ece3c06ca34dd#98b546f8c96347ba81ccb57b5c99a7f1

## 데이터 연산

- 노션확인 : https://www.notion.so/JAVA-1696f11d262347e48e2ece3c06ca34dd#d5607e3422be469683e36935a5315594

→ 비트연산은 복잡한 계산이나 그래픽에서 사용하면 속도가 빠르다 

## 데이터 타입 변환

- 자신보다 큰 타입의 변수에 저장하는 경우
- 연산시 가장 큰 타입으로 변경

→ 강제 형 변환 : (데이터 타입) 변수 또는 값

## 주석문

- 자바 소스에 대한 설명을 추가할 때 사용함
- 종류
    - 한 줄 주석 : //
    - 여러 줄 주석 : /* */

## Annotation

- 일반 주석문과 달리 @로 시작함
- 코드에 대한 설명보다 컴파일러에게 정보를 알려주기 위해 사용함

## API 문서 작성

- 구현이 완성된 프로그램에 대한 사용설명서
- API 문서작성 방법
    - 소스에서 문서 주석을 추가함
    - JAVA_HOME/bin/javadoc.exe 프로그램으로 API 문서를 생성

ex)

```java
package edu;

/**
*@author 이광오
*/
public class Test19{
	/**
	*@param a
	*@param b
	*@return
	*/
	public int sum(int a, int b){
		return a+b;
	}
}
```

## if 문

- 조건의 결과가 true인 경우에 실행할 명령문만 지정

```java
//실행문1
if(조건){
	//실행문2
}
//실행문3
```

## if-else문

- 조건의 결과가 true인 경우와 false인 경우 실행할 명령문 지정

```java
//실행문1
if(조건){
	//실행문2
else{
	//실행문3
}
//실행문4
```

## if-else if문

- 여러 개의 조건에 따라 여러 개의 실행문 지정

```java
//실행문1
if(조건1){
 //실행문2
}
else if(조건2){
	//실행문3
}
else{
	//실행문4
}
//실행문5
```

## Annotation

- 일반 주석문과 달리 @로 시작함
- 코드에 대한 설명보다 컴파일러에게 정보를 알려주기 위해 사용함

## API 문서 작성

- 구현이 완성된 프로그램에 대한 사용설명서
- API 문서작성 방법
    - 소스에서 문서 주석을 추가함
    - JAVA_HOME/bin/javadoc.exe 프로그램으로 API 문서를 생성

ex)

```java
package edu;

/**
*@author 이광오
*/
public class Test19{
	/**
	*@param a
	*@param b
	*@return
	*/
	public int sum(int a, int b){
		return a+b;
	}
}
```

## if 문

- 조건의 결과가 true인 경우에 실행할 명령문만 지정

```java
//실행문1
if(조건){
	//실행문2
}
//실행문3
```

## if-else문

- 조건의 결과가 true인 경우와 false인 경우 실행할 명령문 지정

```java
//실행문1
if(조건){
	//실행문2
else{
	//실행문3
}
//실행문4
```

## if-else if문

- 여러 개의 조건에 따라 여러 개의 실행문 지정

```java
//실행문1
if(조건1){
 //실행문2
}
else if(조건2){
	//실행문3
}
else{
	//실행문4
}
//실행문5
```

## switch문

- 하나의 변수에 값에 대하여 여러 개의 값인지를 판단함

```java
switch(변수){
	case 값1 : 실행문1;
	case 값2 : 실행문2;
	case 값3 : 실행문3;
	case 값4 : 실행문4;
}
```

## 반복문

- for, while, do while
- 체크 사항
    - 몇번을 반복할 것 인가?
    - 반복 횟수를 체크할 변수는 무엇인가?
    - 반복 횟수를 체크할 변수의 초기 값은 무엇인가?
    - 반복 횟수를 체크할 변수의 값은 어떻게 변화할 것인가?
- 반복문 작성 시 반드시 고려해야 할 사항
    - 반복 횟수 변수의 선언 및 초기화
    - 반복할 조건
    - 반복 횟수 변수의 값 변경

## for문

```java
for(변수 선언; 조건식; 증감식){
	실행문
}
```

## while문

```java
변수 선언;
while(조건식){
	실행문;
	증감식;
}
```

## do-while문

```java
변수 선언;
do{
	실행문;
	증감식;
}while(조건식)
```

→break를 통해 반복문을 빠져 나올 수 있다.

→countinue는 현재 실행을 멈추고 다음 반복문을 실행함

## 배열의 장점

- 변수 a→b→c 순서로 접근해야 하는 경우 가장 빠른 접근 방법

→ 배열이란 동일한 타입의 변수들을 순차적으로 메모리에 저장한 후, 첫번째 변수의 메모리 구조값만 이용해 인접한 변수를 접근하는 구조

- .첫번째 변수의 주소(배열에서 주소값 계산할 때 필요한 정보)
- 변수의 주소 : 첫 번째 변수의 주소값 + 인덱스 * 데이터 타입

## 배열의 구현

- 배열을 사용하기 위한 작업 순서
  1. 배열을 메모리에 생성함
  2. 생성된 배열의 시작 주소 값을 변수에 저장함
  3. 인덱스를 이용해 배열 안의 값을 접근함
- 배열 생성
  - 메모리에 동일한 타입의 변수 여러 개를 순차적으로 만듦

    ```java
    new 데이터 타입[변수의 개수];
    ```

  - 배열 주소
    - 배열이 만들어진 시작 주소 값을 변수에 저장함

    ```java
    int[] arr = new int[5];
    ```

- 배열 사용
  - 배열의 시작 주소 값을 가지는 변수와 인덱스를 활용함

    ```java
    //변수이름[인덱스]
    arr[1] = 123;
    int num = arr[1];
    ```

- 배열 초기화 : 배열을 생성한 후 처음 값을 저장 하는 것
  - 배열은 생성과 동시에 자동으로 초기화가 됨
  - 기본 데이터 타입은 0으로 참조 타입은 null로 초기화

    ```java
    int[] score = new int[5];
    int[] socre = {90,80,70,60,50}
    ```

- length

```java
socre.length
```

- 확장  for문

```java
for(int num : arr){
	System.out.println(num);
}
```

- 2차원 배열 선언

```java
new int[5][2]; // new 데이터 타입[행 크기][열 크기]
int[][] arr = new int[5][5];
```

- 2차원 배열 초기화

```java
int[][] arr = {{1,2,3},{4,5,6},{7,8,9}};
```

→2차원 배열은 2중 for문을 사용해서 순회

## 객체지향개요

→ 객체는 속성과 행동으로 구성된다

## 메서드 이름 지정 시 규칙

1. 소문자로 시작하며, 숫자로 시작해서는 안 됨
2. 메서드 기능을 나타낼 수 있는 이름으로 지정함
3. 메소드 이름은 공백을 가질 수 없음
4. 여러 단어가 있는 경우 새로운 단어에서 대문자로 시작하거나 _로 연결함

## 접근제어자

- private : 같은 클래스
- (default) : 같은 패키지
- protected : 같은 패키지 or 상송
- public : 같은 프로젝트

## 오버로딩

- 같은 메서드 네임에 다른 인자 값

## heap 메모리

→ new를 통해 객체(인스턴스)를 heap 메모리에 생성 (개발자 접근 불가) 참조 변수를 통해 주소로 접근 한다.

- 참조변수가 null 값일 경우 오류가 난다

## stack 메모리

- 지역변수가 저장되는 메모리(개발자 접근 가능)

## code 영역

- static 변수가 생성
- 프로그램 실행 전에 생성
- static 블록

```java
//실행전에 블록 실행
static{
...
}
```

## 생성자

→ 멤버 변수를 초기화 하기 위해 사용

## this

- 현재 인스턴스(클래스 객체)를 지정하는 변수
- this()으로 클래스 내에서 생성자 호출 가능

## 상속

- 공통적인 내용이 있을때
- is a 관계가 성립이 될 때
- 상속하는 부모 클래스에 인자값이 없는 생성자는 필수적으로 구현되어 있어야함

## 메서드 오버라이딩

- 상속 받은 메서드 바디만 오버라이딩 가능
- 상속 받은 메서드 선언부는 변경 불가
- 접근 제어자는 동일하거나 큰 범위로 변경 가능

## super keyword

- 상속받은 부모 객체
- super()으로 생성자 호출 가능

## 추상메서드

- abstract 키워드로 추상메서드 생성가능
- 클래스에도 abstract 선언되어야 한다
- 상속받은 자식 클래스에는 무조건 추상메서드의 바디를 구현해야한다
- 상속받은 추상메서드를 자식 메서드에 떠넘기기 위해서는 abstract를 선언하고 자식 클래스에 떠넘길 수 있다

## interface

- 규칙만 정해준다
- 모든 메서드가 추상메서드인 클래스
- class 대신 interface를 사용한다
- new를 통해 변수 생성 불가능 → 컴파일시 public static final이 붙는다
- 컴파일시 abstract가 자동으로 붙는다

## default 메서드

- interface 에서 사용가능
- 자바8부터 활용가능
- 상속받는 모든 클래스에서 공통적으로 가지는 메서드

```java
public default 리턴타입 메서드명(인자값){
	...
}
```

## static 메서드

- 자바8에서 사용가능
- 프로그램 실행전에 메서드를 먼저 구현하여 사용가능

## 다형성

- 내부적으로 모든 클래스의 root는 object이다(extends가 없을 경우 extends Object가 내부적으로 실행)
- heap에 인스턴스를 생성하는 순서는 상위클래스의 object부터 생성한 인스턴스까지 순서대로 만들어진다
- 하위 클래스를 활용하기 위해서는 형변환 해주어야한다.

## instanceof

- 받아온 인스턴스의 타입을 확인하는 문법

## 내부 클래스

- 클래스$클래스로 표현된다
- instant class
- static class

→ new 없이 사용가능 함 하지만 클래스 내부적으로 static이 없는 변수나 메서드를 사용하려면 인스턴스를 생성 해주어야 한다.

- local class

```java
public void method1(){
	class LocalClass{
		... 
	}
}
```

→ 해당 메서드에서만 사용가능하다

- 익명 class

```java
Messenger test = new Messenger(){
	public void setMessage(){
		...
	}

	public String getMessage(){
		...
	}
}
```

## 자바 API(라이브러리)

- [java.io](http://java.io) 입출력
- java.util 유틸(날짜, 시간, 컬렉션)
- java.sql 데이터베이스
- java.lang 프로그램 개발 시 가장 기본 기능

## java.lang

- Object
  - hashCode() → 인스턴스의 고유번호를 확인
  - getClass() →Class 객체를 리턴(class객체는 객체에 대한 정보를 담고 있음)
  - toString() → 고유번호를 16진수로 변환
  - equals() → 객체의 주소값을 비교
- String

  → 문자열 처리에 관련된 클래스

  → 원본은 변경 불가

  - equals() → 문자열 비교
  - equalsIgnoreCase() → 대소문자 관련없이 문자열 비교
  - toString() → 문자열 리턴
  - length() → 길이 출력
  - charAt() → 특정 위치의 문자 리턴
  - trim() → 공백 제거
  - isEmpty() → “”(null string) 판단
  - indexOf() → 인자로 주어진 문자열이 몇번째 인덱스에 위치하는지
  - lastIndexOf() → 인자로 주어진 문자열이 뒤에서 몇번째 인덱스에 위치하는지
  - startWith() → 인자로 주어진 문자열으로 시작하는지
  - endWith() → 인자로 주어진 문자열로 끝나는지
  - concat() → 문자열 합치기
  - replace() → 문자열 치환
  - toLowerCase() → 소문자 변환
  - toUpperCase() → 대문자 변환
  - split() → 특정 인자를 기준으로 문자열 자르기
  - substring() → 인덱스 값을 통해 문자열 자르기
  - valueOf() → 타입을 문자열로 변환하려고 할 때
- StringBuffer(동시접근기능처리) / StringBuilder(동시접근기능처리x)

  → 문자열 처리에 관한 기능을 제공

  → 원본 변경 가능

  - append() →  문자열 붙히기
  - capacity() → 전체 용량
  - delete(int, int) → 범위 삭제
  - deleteCharAt(int) → 지정 삭제
  - insert() → 삽입
  - reverse() → 뒤집기
  - setCharAt(int, char) → 지정 문자 삽입
  - setLength(int) → 길이 변경
  - trimToSize() → 들어있는 문자열로 크기 변경
- Math

  → 수학적인 계산

  - Math.abs() → 절대값
  - Math.ceil() → 정수값(올림)
  - Math.floor() → 정수값(버림)
  - Math.max() → 최대값
  - Math.min() → 최소값
  - Math.pow() → 거듭제곱
  - Math.random() → 랜덤값
  - Math.round() → 정수값(반올림)
  - Math.sqrt() →  제곱근
- Wrapper Class
  - Boolean
  - Charactor
  - Byte
  - Interger
  - Long
  - Double
  - Short
  - Float

  → Wrapper class로 변환 : Boxing

  → 자바5부터 autoboxing 가능


## java.util

- StringTokenizer

  → 문자열 분리하는 클래스

- Random(long seed) : seed값 지정 가능

  → 난수발생 클래스

- Arrays

  → 배열관련 기능 제공

  - binarySearch() → 이진 탐색
  - copyOf() → 복사
  - copyOfRange() → 범위 복사
  - equals([], []) → 인자로 주어진 두 배열을 비교
  - sort() → 배열 정렬
  - toString() → 문자열로 변환
- Date/Calender

  → 날짜 관련 기능 제공

  - month는 0부터 시작이라 +1로 사용
- SimpleDateFormat

  → 날짜의 형식을 정의하는 기능 제공

- MassageFormat

  → 문자열 형식을 정의하는 기능 제공

- DecimalFormat
  - 0: 하나의 숫자를 의미함. 지정된 자리에 숫자가 없으면 0
  - #: 하나의 숫자를 의미함. 지정된 자리에 숫자가 없으면 표현하지 않음
  - .: 소수점
  - -: 음수
