# java_study 이론 입니다.

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
