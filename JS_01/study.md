코딩 자율 학습 Java Script 파트

# 변수와 상수

변수는 값이 변하는 데이터를 저장하고 관리하기 위한 공간으로 변수를 생성함.

## 키워드

어떤 역할이나 기능이 정해진 특별한 언어(예약어)

## 식별자

변수, 함수 등에 부여되는 이름을 의미한다. 변수는 컴퓨터의 메모리라는 곳에 저장.

## 표현식

하나의 값을 반환하는 식 또는 코드를 의미

## 값

더 이상 평가할 수 없는 데이터를 의미

## 선언, 할당

변수의 식별자를 지정하는 행위를 변수를 선언한다고 한다. 연산자인 = 기호로 우변에 있는 값을 변수 공간에 대입하는 것을 값을 할당한다고 한다. 

## 초기화

선언과 할당을 한 번에 하는 것을 변수를 초기화 한다고 한다. 

## let

1. 변수명 중복이 불가능 하다.
2. 호이스팅 되지 않는다.
3. 스코프의 범위가 다르다. 

## 상수 const

1. 변수명 중복이 불가능 하다.
2. 호이스팅 되지 않는다.
3. 스코프의 범위가 다르다.
4. 재할당 불가능 하다. (선언과 할당을 분리하는 것도 불가능)

## 식별자 표기법

카멜 케이스: 변수명과 함수명 작성시 사용 Ex) firstName, lastName
언더스코어 케이스: 상수명 작성시 사용 Ex) FIRST_NAME, last_name
파스칼 케이스: 생성자 함수명 작성시 사용 Ex) FistName, LastName

# 자료형

데이터의 종류를 의미한다. 자료형으로는 string, number, boolean, undefined, null, Symbol, reference(참조), object

## 문자열

탬플릿 문자열은 백틱으로 문자열을 정의하는 방법.

## 숫자형

정수와 실수를 구분하지 않고 전부 하나의 숫자 자료형으로 취급한다. 

## 논리형

true, false를 의미, 연산으로도 구할 수 있다.

## undefined

할당하지 않을 경우 JS 내부적으로 변수와 상수 공간에 임시로 데이터를 할당, 그때의 값이 undefined이다. 

## null

변수나 상수를 선언하고 의도적으로 선언한 공간을 비워 둘 때 할당한다.

## object

파생되는 자료형으로는 배열, 객체 리터럴, 함수가 있다.

### 배열

1. 복수의 데이터를 정의할 수 있는 자료형
2. 배열로 정의한 데이터를 요소라고 한다. 
3. 배열에서 각 데이터가 있는 위치를 가리키는 숫자를 인덱스라고 한다. 
4. 배열은 모든 자료형을 저장할 수 있다. 
5. 비어있는 배열을 정의할 수 있다.

### 객체 리터럴

객체를 정의하는 가장 간단한 방법이며 객체를 정의할 때 중괄호를 사용하며, 중괄호 항에는 키(key), 값(value)의 한쌍으로 이루어진 속성(property)가 들어간다. 
배열과는 다르게 값을 인덱스가 아닌 키로 구분한다. 

# 연산자

= 할당 연산자

## 산술 연산자

수학 연산을 수행하는 연산자를 말한다.

## 비교 연산자

비교 연산자는 피연산자를 비교한 뒤, 논리형 값인 ture와 false를 반환하는 연산을 수핸한다.

== 값이 같으면 true를 반환한다.
=== 값과 자료형이 같으면 ture를 반환한다.
!= 값이 다르면 true를 반환한다.
!== 값과 자료형이 다르면 true를 반환한다.

## 논리 연산자

x && y -> x가 참이면 y를 반환하고 x가 거짓이면 x를 반환
x || y -> x가 참이면 x를 반환하고 x가 거짓이면 y를 반환
!x -> x가 참이면 false를 반환하고 x가 거짓이면 true를 반환

특징: 어떤 피연산자든 모두 논리형으로 평가한다. 

### &&

피연산자를 왼쪽부터 평가해 평가 결과가 거짓이면 거짓이 나온 피연산자를 즉시 반환하고, 거짓이 아니면 마지막 피연산자를 반환한다.

### ||

피연산자를 왼쪽부터 평가해 참으로 평가된 피연산자를 즉시 반환한다. 만약 모든 피연산자가 참으로 평가되지 않으면 마지막 피연산자를 반환

## 삼항 연산자

세 항 중 가장 왼쪽에 있는 피연산자의 참, 거짓에 따라 나머지 두 항에 있는 피연산자를 선택적으로 반환하는 연산을 수행한다. 