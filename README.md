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