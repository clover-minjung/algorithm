# qr code

문제 바로가기: [qr code](https://school.programmers.co.kr/learn/courses/30/lessons/181903)

<br/>

## **🔍 문제 설명**

두 정수 `q`, `r`과 문자열 `code`가 주어질 때, `code`의 각 인덱스를 `q`로 나누었을 때 나머지가 `r`인 위치의 문자를 앞에서부터 순서대로 이어 붙인 문자열을 return 하는 solution 함수를 작성해 주세요.

<br/>

### **✅ 제한사항**

- 0 ≤ `r` < `q` ≤ 20
- `r` < `code`의 길이 ≤ 1,000
- `code`는 영소문자로만 이루어져 있습니다.
<br/>

### **입출력 예**


| q | r |        code        |    result     | 
|---|---|--------------------|---------------|
| 3 | 1 | "qjnwezgrpirldywt" |     "jerry"   |
| 1 | 0 |   "programmers"    | "programmers" |

**예 1)**
예제 1번의 `q`와 `r`은 각각 3, 1이고 인덱스와 그 값을 `q`로 나눈 나머지가 1인 인덱스의 문자들을 앞에서부터 순서대로 이어 붙이면 "jerry"가 되므로 이를 return 합니다.

<br/>

## **🔍 CODE REVIEW**
<br/>

### **🖥️ 제출 코드**

```python
def solution(q, r, code):
    answer = ''
    for i in range(len(code)):
        if i % q == r:
            answer += code[i]
    return answer
```

#### **📍풀이**

- 문자열을 저장할 변수 `answer` 초기화
- `code`의 인덱스에 접근하기 위해서 반복문 사용
- 인덱스를 `q`로 나누었을 때 나머지가 `r`인 위치의 문자 `answer`에 더하기
- 최종 `answer` 값 반환

<br/>

### **💡다른 코드**
```python
def solution(q, r, code):
    return ''.join([code[i] for i in range(len(code)) if i % q == r])
```

#### **📍풀이**

- `join()`과 리스트 컴프리헨션을 이용해 제출 코드를 간소화

<br/>

```python
def solution(q, r, code):
    answer = ""
    for i, char in enumerate(code):
        if i % q == r:
            answer += char
    return answer
```

#### **📍풀이**

- 제출 코드와 같은 풀이
- 인덱싱이 아닌 `enumerate()`를 사용해서 문자열의 인덱스와 각 문자를 직접 변수로 받음
- `i`(인덱스)를 `q`로 나누었을 때 나머지가 `r`인 문자 `char`를 빈 문자열에 더하기
- 최종 문자열 `answer` 값 반환
<br/>

  #
### **🗒️ 정리**
✒️ 인덱싱   
✒️ `join()` 함수   
✒️ `enumerate()` 함수