# 문자열의 뒤의 n글자

문제 바로가기: [문자열의 뒤의 n글자](https://school.programmers.co.kr/learn/courses/30/lessons/181910)

<br/>

## **🔍 문제 설명**

문자열 `my_string`과 정수 `n`이 매개변수로 주어질 때, `my_string`의 뒤의 `n`글자로 이루어진 문자열을 return 하는 solution 함수를 작성해 주세요.

<br/>

### **✅ 제한사항**

- `my_string`은 숫자와 알파벳으로 이루어져 있습니다.
- 1 ≤ `my_string`의 길이 ≤ 1,000
- 1 ≤ n ≤ `my_string`의 길이
<br/>

### **입출력 예**

|      my_string   |  n |     result    |
|------------------|----|---------------|
| "ProgrammerS123" |  11| "grammerS123" |
|    "He110W0r1d"  |  5 |    "W0r1d"    |

**예 1)**
예제 1번의 my_string에서 뒤의 11글자는 "grammerS123"이므로 이 문자열을 return 합니다.

<br/>

## **🔍 CODE REVIEW**
<br/>

### **🖥️ 제출 코드**

```python
def solution(my_string, n):
    return my_string[-n:]
```

#### **📍풀이**

- 슬라이싱을 이용해 문자열의 뒤의 `n` 글자로 이루어진 문자열 반환
- 슬라이싱에서 `-`는 역순을 의미, 따라서 `[-n:]`는 -n값 부터 문자열의 끝까지를 나타냄

<br/>

  #
### **🗒️ 정리**
✒️ 슬라이싱
