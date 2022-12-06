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

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ee54c0ba-2cd3-40fe-aebc-dd2bafe2390c/Untitled.png)

4) 실수 타입 :

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/308eefa4-5868-4c38-9e49-00ffec2fcd06/Untitled.png)

5) 참조 타입 :

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5501e71a-b8ea-4d0f-95dd-28047dabcbfd/Untitled.png)

## 데이터 연산

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7722d49e-9eba-468e-869a-c7e6799c0a7e/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4e66a837-151b-44fa-a8f5-afaf1c2c01f7/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/83a061a3-499b-4ef5-8a97-49f58fb520c8/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/87139bef-7cbc-447a-b20e-78d30b74cb1a/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/34a6ff5e-f590-4d7a-97f4-de436e4e6a20/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/bc686b5e-92fc-44c0-835c-3bba1a45d1ea/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a98aa0dc-84f5-4ff6-8a6e-e464901577e9/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e7fd3b1f-88d9-45fe-b413-da5dc550d763/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/bc0b8a80-5751-41e3-9c2f-dd03c40d7d5e/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/75f659ea-f3fb-49d5-9cf6-09215cfc32c4/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/bf0efff5-9f7e-4855-8615-464a7c2c36ac/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/93aff47f-4fd6-4a50-b38f-bbd2f0c584bf/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/09fc93bf-3194-4698-a2de-1f9e1813eeca/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/48a3a5c7-45f7-4227-b926-a783ea5de1cb/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b6519748-e9be-461c-96d5-30599ccf6368/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f9cb56d4-d627-4fe4-a5dc-53c2125940aa/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1ac2078d-bd7e-487f-a02a-e48e4382616d/Untitled.png)

→ 비트연산은 복잡한 계산이나 그래픽에서 사용하면 속도가 빠르다