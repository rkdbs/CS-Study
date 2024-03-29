[자료구조] 스택(Stack), 큐(Queue)
=

### 개요
스택과 큐는 모두 데이터를 임시 저장하기 위해 사용하는 자료구조이다. 데이터를 입력하고 출력하는 방향이 있으며, 유사한 점을 많이 가지고 있다.

> 스택(Stack)

### 정의
최근에 저장한 데이터를 먼저 사용하는 구조로 LIFO(Last In First Out) 구조라고 칭한다.

### 용어
- push(): 스택에 데이터를 삽입하는 작업
- pop(): 스택의 top에서 데이터를 꺼내는 작업
- overflow(): limit을 벗어나면 발생
- limit: push할 수 있는 한계로 배열의 끝
- top: 데이터 상단
- base: 스택의 시작 위치로 가장 아래(index 0)
- underflow: base를 벗어나면 발생(index -1 이하)

### 사용 예시
- 브라우저 방문기록
- 역순 문자열 만들기
- 실행 취소
- 후위 표기법 계산
- 수식 괄호 검사

> 큐(Queue)

### 정의
먼저 저장한 데이터를 먼저 사용하는 구조로 FIFO(First In First Out) 구조라고 칭한다.

### 용어
- add(): 데이터를 추가하는 작업
- delete(): 데이터를 꺼내 사용하는 작업
- rear: 가장 최근에 추가한 데이터를 지시하는 포인터/인덱스
- front: 사용할 데이터를 지시하는 포인터/인덱스
- overflow: 끝까지 add()된 경우
- underflow: 더 이상 꺼낼 수 없는 경우

### 종류
- 선형 큐(Linear Queue)
- 환형 큐(Circular Queue)
- 데큐(DeQueue)
- 우선순위 큐

### 사용 예시
- 우선 순위가 같은 작업 예약(프린터 인쇄 대기)
- 은행 업무
- 콜센터 대기 시간
- 프로세스 관리
- 너비 우선 탐색
- 캐시

## 정리
||스택|큐||
|---|---|---|---|
|정의|먼저 들어온 데이터가 먼저 나가는 구조(FIFO)|마지막에 들어온 데이터가 먼저 나가는 구조(LIFO)||
|삽입/삭제|push/pop|enqueue/dequeue||
|장점|구현 쉬움, 메모리 관리 용이|데이터의 순서가 중요한 작업에 적합||
|단점|데이터 접근의 어려움, 중간에 있는 데이터에 접근하려면 맨 위의 데이터부터 차례로 꺼내야함|큐의 크기가 고정되어 있으면 데이터가 가득 차 더 이상 삽입 불가능||