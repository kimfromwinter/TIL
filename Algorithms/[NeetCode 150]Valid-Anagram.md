# [NeetCode 150] Array and Hassing #2

### **Valid Anagram**

두 문자열이 서로 애니어그램이면 True 값을, 아니면 False 를 반환

### ***main theme**

파이썬의 내장함수 sorted() 를 사용한다.

(이때, sorted의 결과로는 무조건 리스트형을 반환한다는 것에 주의)

and

Brute Force 알고리즘을 이용한다.

```python
class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        if (sorted(s) == sorted(t)) :
            return True
        else :
            return False
```

두 주어진 문자열을 정렬한 뒤 직접 비교한다.

⇒ O(n logn), O(n)
