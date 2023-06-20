# 자료형

::: tip
- 코드에서 변수가 필요한 이유는?
- 상수도 메모리에 저장될까?
:::

- 파이썬에서 **식별자(변수명)** 에 값을 할당해서 변수를 생성한다. 
- `code` 상에서 작성된 변수는 실행 시에 변수에 할당된 값을 의미한다.
- **할당(`=`) 연산자**의 왼쪽에 표현된 변수 이름은 메모리 공간을 의미한다.

::: warning
- 파이썬에서 사용중인 **keyword** 들은 식별자(변수명, 함수명)로 사용하지 않는다.
:::


## 파이썬의 자료형_data type

- 변수에 저장되는 값에 의해 **자료형(type)** 이 결정된다.

```python
val = True      # boolean
val = 1         # integer
val = 3.14      # float
val = 'python'  # string
val = None      # None
val = [1, 2, 3] # list
val = {}        # dictionay
val = (1, 2)    # tuple
```

- **컨테이너** 자료형들은 생성함수들을 사용할 수 있다.

```python
val_list = list() 
val_set = set()
val_dict = dict()
```

## 연산자 operator

- 연산자는 컴퓨터에 명령을 할 수 있는 가장 작은 계산 작업이다.
- 자료형에는 사용할 수 있는 연산자들이 정해져 있다.
- 피연산자의 자료형에 의해 달리 동작하는 연산자들이 있다. 

::: tip
- 단항 연산자가 이항 연산자보다 우선 순위가 높다.
- 할당 연산자는 마지막에 실행된다.
- 리스트 인덱스, 함수 호출, 슬라이싱은 우선순위가 높다.
- 사칙연산자 > 비트 연산자 > 비교 연산자 > 논리 연산자
:::

## 수식 expression

- 상수, 혹은 변수만 작성해도 수식이 된다.
- 함수는 값을 반환하면 **함수 호출** 도 수식이다.
- 수식은 하나의 값으로 계산(평가)된다.


## 형변환 type conversion

- **암시적 형변환** : 파이썬 인터프리터가 수행
  - *이항 연산자* 에 적용된 피연산자들의 자료형이 다르면 형변환을 시도한다.

- **명시적 형변환** : 프로그래머가 의도적으로 수행

## 추가 참고

- `boolean` 자료형이 아니라도 **논리 연산** 이나 `bool()` 에 적용된 값들은 `True/False` 로 변환  
  - `0`, `0,0`, `None`, `[]`, `()`, `{}` ==> **`False`**
  - 그 외는,  **`True`**

- 단축평가
```python
print(0.0 or 1.1)     # 1.1
print(None and [])    # None
```


<!-- @[code](./codes/10_03_writetext.py) -->
