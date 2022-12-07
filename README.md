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