# 활동 01 과제

# 자바 기본 프로그래밍

## 자바의 데이터 타입

### 데이터 타입이란?
자료형. 변수명 앞의 int, String 등. 변수의 앞에 쓰여 변수의 자료형을 지정해줌. 자바의 데이터 타입의 크기는 CPU나 운영체제에 따라 **변하지 않는다.**

### 자주 쓰이는 자료형
- int
- long
- double
- boolean
- char
- String
- StringBuffer
- List
- Map
위와 같은 primitives type이 있고 아래처럼 사용자 정의 자료형도 있다.
> class Animal {<br>
  psvm{Animal cat;}<br>
}


### 레퍼런스 타입
primitives type과 다른 형태로 references type이 있다. 레퍼런스 타입에는 배열 타입, 열거 타입, 클래스, 인터페이스 등이 있다.

### 자바의 데이터 타입
![자바 데이터 타입](https://t1.daumcdn.net/cfile/tistory/9990144E5AB240FC20)


## 상수

### 상수 선언
상수 선언 시 주의사항은 아래와 같다.
- final 키워드 사용
> final double PI = 3.141592;

- 선언 시 초기값 지정
- 실행 중 값 변경 불가
상수 이름은 보통 **모든 문자를 대문자**로 표시한다.



# 반복문과 배열 그리고 예외처리

## main() 메소드 원형
main() method의 형태는 아래와 같다.
> public static void main(String[] args)

자바도 C와 마찬가지로 가장 먼저 시작하는 시작점. Entry point가 있다. C의 main()함수처럼 자바는 main()메소드가 있다. 
> public

public은 공개 범위를 나타낸다. 이 위치에는 public, protected, private가 올 수 있다. 하지만 public이 아닌 것으로 지정할 경우 다른 클래스로부터의 접근에 문제가 생겨 main으로서의 기능을 상실하므로 public으로 지정한다.
> static

static은 프로그래밍이 시작한 후에 따로 인스턴스 하지 않아도 시작과 동시에 메모리에 호출이 된다. (JVM의 GarbageCollector로 인해 클래스, 메소드, 변수 등은 일정 용도를 끝마친 후에 메모리에서 삭제가 되거나 다른 부분에서 참조가 되지 않는다.)
> void

메소드에 return 값이 없다는 뜻이다. 이유는 C언어에서와 같다.
> String[] args

프로그램이 시작되자마자 받는 특정한 값을 String type의 배열에 저장해 프로그램 안에서 사용할 수 있다. 프로그램의 실행 순간, 외부값을 가져와서 프로그램 안에 사용하고자 할 때 메모리에 저장할 공간을 미리 선언해 두는 것이라고 할 수 있다.<br>
문자열 이름은 꼭 args일 필요는 없다.


# 클래스와 객체

## 

### 객체와 인스턴스의 차이
클래스에 의해 만들어진 객체를 인스턴스라고도 한다. 그렇다면 객체와 인스턴스의 차이는 무엇인가. 
> Animal cat = new Animal(); 

이렇게 만들어진 cat은 객체이다. 그리고 cat이라는 객체는 Animal의 인스턴스이다. 즉 인스턴스라는 말은 특정 객체 cat 이 어떤 클래스 Animal의 객체인지를 관계위주로 설명할 때 사용된다. 즉, cat은 객체 ( ~~cat은 인스턴스~~ ), cat은 Animal의 인스턴스 ( ~~cat은 Animal의 객체~~ ).


## 기본 생성자

### 생성자를 만들지 않았을 때 생기는 기본 생성자는 보이지 않는다. 컴파일러가 만들고 실행해주기 때문에 컴파일러 이전에 있는 코드에는 변화가 없음.

# 궁금한 점
## 예제 3-17
- [ ]
예제 3-17의 16행 
> scan.next();

부분에서 입력 스트림에 있는 정수가 아닌 토큰을 버린다고 하는데 작동원리가 궁금함. 
[이거인듯](https://medium.com/@kimddub/java-scanner-%EB%B2%84%ED%8D%BC-%EB%B9%84%EC%9A%B0%EA%B8%B0-913c652cc144)