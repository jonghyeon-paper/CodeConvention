# CodeConvention

### 명명규칙
> 0. 공통사항.
> + 
>
> 1. 파일명.
> + 파스칼표기법을 사용한다. 
> + 명사로 표현한다.
> + 
>
> 2. 변수
> + 카멜 표기법을 사용한다.
> + 명사로 표기한다.
> + 
>
> 3. 상수
> + 언더스코어 표기법(스네이크 표기법)을 사용한다.
> + 모든 문자는 대문자를 사용한다. 
> + 
>
> 3. 함수(메소드)
> + 카멜 표기법을 사용한다.
> + 첫 시작은 동사를 사용한다.
> + 자주 사용하는 동사
>   + get, set
>   + retrieve,  add, edit, remove
>   + update
>   + 
>

### 프로그래밍 규칙
> 0. 공통사항.
> + 
> + 조건문(if, else if, case).
> 조건문의 사용시 중첩이 3번 이상 발생하는 경우 부정조건으로 작성한다.
>
<pre>
if (a == 1) {
	if (b == 2) {
		if (c == 3) {
			...
		}
	}
}

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
</pre>
>
> + 반복문.
> + 함수형 프로그래밍.
> + 변수변위.
> + 전역변수.
> + 가동성.
> + 



 