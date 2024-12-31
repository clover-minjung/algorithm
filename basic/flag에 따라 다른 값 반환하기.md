# flag에 따라 다른 값 반환하기

문제 바로가기: [flag에 따라 다른 값 반환하기](https://school.programmers.co.kr/learn/courses/30/lessons/181933)

<br/>

## **🔍 문제 설명**

두 정수 `a`, `b`와 boolean 변수 `flag`가 매개변수로 주어질 때, `flag`가 true면 `a` + `b`를 false면 `a` - `b`를 return 하는 solution 함수를 작성해 주세요.

<br/>

### **✅ 제한사항**

- -1,000 ≤ `a`, `b` ≤ 1,000
<br/>

### **입출력 예**

|  a | b | flag | result |
|----|---|------|--------|
| -4 | 7 | true	|    3   |
| -4 | 7 | false|	 -11   |

**예 1)**
예제 1번에서 flag가 true이므로 a + b = (-4) + 7 = 3을 return 합니다.

<br/>

## **🔍 CODE REVIEW**
<br/>

### **🖥️ 제출 코드**

```python
def solution(a, b, flag):
    return a + b if flag else a - b
```

#### **📍풀이**

- `flag`가 trun면 a+b, 아니면 a-b 반환
- `if elif`문으로 `flag`의 조건을 명확하게 지정할 수도 있음

<br/>

  #
### **🗒️ 정리**
✒️ 삼항연산자
