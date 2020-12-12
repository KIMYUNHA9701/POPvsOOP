# POPvsOOP

## 1.	절차지향과 객체지향의 개념과 특성
  절차지향은 순차적인 처리가 중요하고 프로그램 전체가 유기적으로 연결되도록 만드는 프로그래밍 기법이다. 대표적인 절차지향 언어에는 C언어, 파스칼, 코볼, 포트란 등이 있다. 절차 지향 방식은 컴퓨터의 작업 처리 방식과 유사하기 때문에 처리 시간이 빠르다. 그리고 메모리를 직접 조작할 수 있다. 단점으로는 ‘유지보수가 어렵다’, ‘실행 순서가 정해져 있으므로 코드의 순서가 바뀌면 다른 결과가 나올 수 있다’, ‘디버깅이 어렵다’는 점이 있다.
객체지향은 실제 세계를 모델링하여 소프트웨어를 개발하는 방법이다. 개발하려는 것을 기능별로 묶어 모듈화함으로써 하드웨어가 같은 기능을 중복으로 연산하지 않도록 하고, 모듈을 재활용하기 때문에 하드웨어의 처리양을 획기적으로 줄어준다. 대표적인 객체지향 언어에는 Java, C++, Python 등이 있다. 
객체지향의 특징에는 캡슐화, 상속, 다향성이 있다. 캡슐화는 관련된 데이터와 알고리즘(코드)이 하나의 묶음으로 정리된 것으로 사용이 편리하다. 상속은 이미 작성된 클래스를 이어받아 새로운 클래스를 생성하는 기법으로 코드 재사용할 수 있다. 다형성은 동일한 작업을 하는 함수들에게 똑같은 이름을 부여할 수 있으므로 코드가 간단해진다. 이러한 특징들로 인한 신뢰성 있는 소프트웨어를 쉽게 작성할 수 있다, 코드를 재사용할 수 있다, 업그레이드가 쉽다, 그리고 디버깅이 쉽다는 장점이 있다. 단점으로는 처리속도가 느리다, 설계에 많은 시간이 소요된다, 어떤 모듈의 한 기능만 필요하더라도 모듈 전체를 가져와야 하기 때문에 프로그램 사이즈가 더 커질 수도 있다는 점이 있다. 
 
****
## 2.	객체지향 관련 용어 정리

#### 1. 클래스(Class)
 흔히 객체의 청사진(Blueprint) 이라고 많이 정의한다.  "상태" 와 "행위" 를 갖는 자바의 기본 단위이다. 한 마디로 건물(객체)을 지을 때 필요한 설계도라고 생각하면 된다. 완성된 건물이 자바에서는 객체(Object) 이다.

#### 2. 상태(State)와 행위(Behavior)
 어떤 사물을 나타낼 때에는 상태와 행위로 구분하여 표시하는 것이 가능하다. 자바에서 "상태"는 클래스나 인스턴스 변수로, "행위"는 메서드로 표현할 수 있다.

#### 3. 객체(Object)
 객체 지향 프로그래밍의 기본 단위로 데이터(실체) 변수(상태)와 메서드(행위)를 모두 포함하고 있다. 클래스는 사물의 단위를 의미하지만, 객체는 각 사물을 의미한다. 예를 들면, 책은 클래스이고 <Java의 정석>은 객체라고 볼 수 있다.

#### 4. 인스턴스(Instance)
 한 클래스의 특정한 객체를 의미한다. 일반적으로 어떤 집합에서 그 집합의 개별적인 요소를 인스턴스라고 한다.

#### 5. 인스턴스화 
 클래스에서 인스턴스를 생성시키는 것을 말한다. 자바에서 new를 사용해 클래스를 복제하여 새로운 객체를 생성하는 것을 흔히 인스턴스화라고 한다.

#### 6. 생성자와 소멸자
 객체는 생성되고 소멸될 때 호출되는 특별한 메서드를 가지고 있다. 이 메서드를 생성자와 소멸자라고 한다. 생성자는 객체를 초기화하거나 설정하고 소멸자는 객체를 삭제하고 정리한다. 

#### 7. 멤버
 객체 혹은 클래스의 변수나 메서드를 의미한다.

#### 8. 변수(Variable)
 값이 저장된 기억장소(메모리). 객체는 변수에 자신의 상태를 저장하고, 변수는 식별자로 명명된다. 

#### 9. 식별자(Identifier)
 프로그래머가 프로그램에서 사용하는 자료의 항목, 즉, 변수, 함수, 상수, 배열, 클래스, 메서드 등에 부여하는 이름을 말한다.

#### 10. 메서드(Method)
 메서드는 특정한 일을 수행하는 행위나 동작을 의미한다. 일반적으로 함수와 같은 의미지만 객체지향에서는 차이점이 있다. static(Class) 메서드와 instance 메서드 2종류가 있으며, static 메서드는 객체를 생성하지 않아도 사용할 수 있지만, instance 메서드는 객체를 생성해야만 사용 가능하다.

#### 11. 멤버 변수
 클래스나 객체의 멤버로 클래스 내에서 선언된 변수를 멤버변수라 한다. 멤버변수에는 static(Class) 변수와 instance 변수가 있으며 static(Class) 변수는 모든 객체가 공통적으로 사용하는 변수이며, instance 변수는 각 객체들마다 따로 생성되어 개별적으로 사용하는 변수이다.
 * 지역변수는 메서드 내에서 선언되어 메서드 내부에서만 사용 가능한 변수를 말하며, 멤버 변수는 메서드나 생성자 바깥에 선언되어야 하며 클래스 전체 영역에서 사용하는 변수를 말한다.

#### 12. 멤버 함수
 클래스 내에서 선언된 함수를 말하며, 멤버 변수들을 통제하기 위하여 사용한다. public, protected, private와 같은 접근 제한자를 사용한다.

#### 13. 접근 제한자
 1) public: 모든 접근을 허용
 2) protected: 같은 패키지에 있는 객체와 상속관계의 객체들만 허용 
 3) default: 같은 패키지에 있는 객체들만 허용
 4) private: 현재 객체 내에서만 허용

****

## 3.	결론
  게임을 만들 때 보통 객체지향 프로그래밍을 채택한다. 게임 제작 시간을 많이 단축해주기 때문이다. 그렇다면 객체지향 프로그래밍이 절차지향 프로그래밍보다 나은가? 그렇지 않다. 프로젝트가 커지면 객체지향의 속도는 느려진다. 객체지향은 표면상으로 보기에는 아주 단순한 기능이지만 뒤에서는 아주 복잡한 일들이 일어나고 있는 경우가 있다. 원하는 기능이 있을 때 객체지향은 구현이 되어있는 코드 뭉치들이 라이브러리화되어 제공되는 것이기에 사용하는 프로그래머 입장에선 굉장히 편하고 시간이 단축된다. 하지만 개개인의 입맛에 맞춰 최적화해주기 어렵다. 절차지향은 백지부터 시작해야하지만 프로그래머의 입맛대로 최적화하고 설계할 수 있다. 따라서, 프로그래머의 실력이 훌륭하다면 객체지향 기능을 사용했을 때보다 더 빠른 성능을 내는 코드를 작성할 수도 있다. 따라서, 임베디드 시스템과 같은 분야에서는 절차지향 프로그래밍을 선호한다. 한정된 자원에 맞춰 세밀한 부분까지 최적화할 수 있는 여지를 주기 때문이다.
그렇다면 어떤 것이 더 나은 프로그래밍 방법인가? 결론은 둘 사이에 우열을 가릴 수는 없다는 것이다. 각 언어들의 특성을 잘 파악하고 그때그때 상황에 맞게 다루는 것이 가장 좋은 방법이다. 따라서, 프로그래머에겐 그것을 파악하고 잘 다룰 수 있는 실력이 필요하다.

