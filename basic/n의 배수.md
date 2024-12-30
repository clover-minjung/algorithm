# n의 배수

문제 바로가기: [n의 배수](https://school.programmers.co.kr/learn/courses/30/lessons/181937)

<br/>

## **🔍 문제 설명**

정수 `num`과 `n`이 매개 변수로 주어질 때, `num`이 `n`의 배수이면 1을 return `n`의 배수가 아니라면 0을 return하도록 solution 함수를 완성해주세요.

<br/>

### **✅ 제한사항**

- 2 ≤ `num` ≤ 100
- 2 ≤ `n` ≤ 9
<br/>

### **입출력 예**

| num | n | result |
|-----|---|--------|
|  98 |	2	|    1   |
|  34	| 3	|    0   |

**예 1)**
98은 2의 배수이므로 1을 return합니다.

<br/>

## **🔍 CODE REVIEW**
<br/>

### **🖥️ 제출 코드**

```python
def solution(num, n):
    return 1 if num % n == 0 else 0
```

#### **📍풀이**

- `num`을 `n`으로 나눈 나머지가 0이면(`num`이 `n`의 배수이면) 1 반환, 아니면 0 반환

<br/>

### **💡다른 코드**

```python
def solution(num, n):
    return int(num % n == 0)
```

#### **📍풀이**

- `num`을 `n`으로 나눈 나머지가 0이면 True를 반환하므로 정수형으로 변환해서 1 반환
- 나머지가 0이 아니면 False를 반환하므로 0 반환
<br/>

  #
### **🗒️ 정리**
✒️ 나머지 연산자 `%`    
✒️ 정수형 변환 `int()`
