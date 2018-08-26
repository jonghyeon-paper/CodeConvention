# CodeConvention

### 명명규칙
0. 기본사항.
+ 풀네임을 사용한다.
+ 목록형 ~List 사용.
+ 배열형 ~s(복수형 표기) 사용.
+ 단일형 ~Data 사용.
+ 구조형(structure) 또는 계층형(hierarchy) ~Information(Info) 사용.
+ 트리형 ~Tree 사용.(계층형과 다른점은 동일한 구조의 데이터가 계층형태)

1. 파일명.
+ 파스칼표기법을 사용한다. 
+ 명사로 표현한다.

2. 변수
+ 카멜 표기법을 사용한다.
+ 명사로 표기한다.

3. 상수
+ 언더스코어 표기법(스네이크 표기법)을 사용한다.
+ 특수한 목적으로 사용한다.
+ 반복되어 표현되는 데이터로 사용한다.

3. 함수(메소드)
+ 카멜 표기법을 사용한다.
+ 첫 시작은 동사를 사용한다.
+ 자주 사용하는 동사
  + get, set
  + retrieve,  add, edit, remove
  + update
  + 




***




### 프로그래밍 규칙

+ 조건문(if, else if, case). 조건문 사용 시 중첩이 3번 이상 발생하는 경우 부정조건으로 작성한다.

<pre>
if (a == 1) {
	if (b == 2) {
		if (c == 3) {
			// TODO true process
			...
		}
	}
}

// 부정조건으로 변경

if (a != 1) {
	// out
}
if (b != 2) {
	// out
}
if (c != 3) {
	// out
}
// TODO true process
...
</pre>

+ 반복문. 반복문의 복잡도는 O(N^2)를 초과하지 않도록 한다.

+ 함수형 프로그래밍. 함수형 프로그래밍이 나쁜 건 아니다다. 하지만 무조건적인 함수형 프로그래밍은 가동성을 떨어뜨릴 수 있고, 프로세스 흐름을 파악하기 어렵게 한다. 또 잦은 문맥교환을 발생시킨다.(이는 재귀함수의 단점이기도 하다.) 프로세스의 흐름을 알고 흐름데로 프로그래밍하되 두 번 이상 같은 프로세스가 실행되는 경우, 가동성을 해치지 않는 선에서 함수형 프로그래밍을 사용한다.

+ 변수변위. 변수 선언시 변수의 라이프사이클을 고려해라. 전역변수, 지역변수, 임시변수 등 용도에 따라서 변수에도 라이프사이클이 있다. 프로세스가 실행되고 종료되기 전까지 사용되는 전역변수가 있는가하면, 0.1초 동안만 사용되는 임시변수도 존재한다. 무분별한 전역변수는 가독성을 해치고 프로세스 흐름을 알기 어렵게 한다. 또한 같은 용도로 임시변수를 남발하면 아니쓰는것만 못하다. 일반적으로 변수는 지역변수라고 생각하고 선언한다. 그 이후에 메소드, 클래스, 프로세스 등 범위를 고려하여 변수의 범위를 확장해라.

+ 클래스 설계. 클래스 설계 시 클래스의 범위를 확정한다. 해당 클래스에서 수행해야할 기능과 그렇지 않은 기능을 명확하게 한다. 기본적으로 생성자 및 메소드에 전달되는 파라미터는 무결하다는 전제로 설계한다. 사용자로부터 입력받는 값이 아니라면 파라미터값은 무결해야한다.

+ primitive타입 변수. 필수로 값이 존재하는 변수인 경우 primitive로 선언한다. 그 외에는 오브젝트타입 변수를 사용한다. null이 허용되는 변수인지 확인해라. 잘 모르겠다면 오브젝트 타입을 사용해라. primitive타입의 변수는 null이 허용되지 않기 때문에 초기화를 하지 않아도 값을 가지고 있다. 이 경우 프로그래머의 의도와 다르게 동작할 수 도 있다.

+ 오브젝트타입 변수.

+ 변수 초기화. 변수 초기화가 필요한경우 null로 초기화한다. primitive타입인 경우 0으로 초기화한다.

+ 매개변수를 로컬변수에 재할당 금지. 생성자를 재외하고는 매개변수를 로컬변수에 재할당 하지 않는다. 특히 로컬 전역변수에는 더욱 재할당 하지 않는다. 매개변수로 받은 값을 어떠한 계산도 없이 로컬 변수에 재할당하면 변수만 낭비된다. 전역변수에 재할당하면 전역변수의 값의 흐름을 파악하는데 어렵게 된다.

+ 오브젝트타입의 매개변수를 로컨변수에 재할당 금지. 전역변수에 재할당하면 전역변수의 값의 흐름을 파악하는데 어렵게 된다. JAVA에서 메소드(함수)는 call by value로 동작한다. 하지만 매개변수가 오브젝트이면(원시타입은 제외) call by reference처럼 동작한다. 때문에 의도하지 않은 값의 변화가 발생할 수 있다.

+ 전역변수.

+ 가독성.

+ 
+ 
+ 
+ 
