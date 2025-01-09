# rny_string

문제 바로가기: [rny_string](https://school.programmers.co.kr/learn/courses/30/lessons/181863)

<br/>

## **🔍 문제 설명**

'm'과 "rn"이 모양이 비슷하게 생긴 점을 활용해 문자열에 장난을 하려고 합니다. 문자열 `rny_string`이 주어질 때, `rny_string`의 모든 'm'을 "rn"으로 바꾼 문자열을 return 하는 solution 함수를 작성해 주세요.

<br/>

### **✅ 제한사항**

- 1 ≤ `rny_string`의 길이 ≤ 100
- `rny_string`은 영소문자로만 이루어져 있습니다.
<br/>

### **입출력 예**

|   rny_string  |     result      |
|---------------|-----------------|
| "masterpiece" | "rnasterpiece"  |
| "programmers" | "prograrnrners" |
|     "jerry"   |	     "jerry"    |
|     "burn"    |      "burn"     |

**예 1)**
예제 1번의 rny_string의 'm'을 "rn"으로 바꿔 "rnasterpiece"를 return 합니다.

<br/>

## **🔍 CODE REVIEW**
<br/>

### **🖥️ 제출 코드**

```python
def solution(rny_string):
    return rny_string.replace('m', 'rn')
```

#### **📍풀이**

- `replace()`를 이용해 문자열의 모든 문자 'm'을 'rn'으로 바꿔준 후 바로 반환
- `replace()`는 문자열 내에 있는 모든 문자를 대체

<br/>

  #
### **🗒️ 정리**
✒️ `replace()`함수
