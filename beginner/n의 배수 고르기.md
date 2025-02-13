# n의 배수 고르기 

문제 바로가기: [n의 배수 고르기](https://school.programmers.co.kr/learn/courses/30/lessons/120905)

<br/>

## **🔍 문제 설명**

정수 `n`과 정수 배열 `numlist`가 매개변수로 주어질 때, `numlist`에서 `n`의 배수가 아닌 수들을 제거한 배열을 return하도록 solution 함수를 완성해주세요.

<br/>

### **✅ 제한사항**

- 1 ≤ n ≤ 10,000
- 1 ≤ `numlist`의 크기 ≤ 100
- 1 ≤ `numlist`의 원소 ≤ 100,000
<br/>

### **입출력 예**


| n |            numlist             |       result       |
|---|--------------------------------|--------------------|
| 3 | [4, 5, 6, 7, 8, 9, 10, 11, 12] |     [6, 9, 12]     |
| 5 |      [1, 9, 3, 10, 13, 5]      |      [10, 5]       |
| 12|    [2, 100, 120, 600, 12, 12]  | [120, 600, 12, 12] |

**예 1)**
`numlist`에서 3의 배수만을 남긴 [6, 9, 12]를 return합니다.

<br/>

## **🔍 CODE REVIEW**
<br/>

### **🖥️ 제출 코드**

```python
def solution(n, numlist):
    a = []
    for i in numlist:
        if i % n == 0:
            a.append(i)
    return a
```

#### **📍풀이**

- `n`의 배수가 아닌 수들을 제거한 배열을 저장할 리스트 `a` 초기화
- `for`문을 사용해 `numlist`의 각 요소들을 가져와 `n`의 배수인 수를 `a`에 추가
- 최종 `a` 반환

<br/>

### **💡다른 코드**
```python
def solution(n, numlist):
    return [i for i in numlist if i % n == 0]
```

#### **📍풀이**

- 제출 코드를 리스트 컴프리헨션으로 풀이
<br/>

  #
### **🗒️ 정리**
✒️ `append()` 함수   
✒️ 리스트 컴프리헨션