# [NeetCode 150] Array and Hassing #1

### Contains Duplicate

: 리스트 안에서 중복되는 숫자가 있을 때 True, 중복이 없을 때 False 를 반환

---

### ***main theme**

파이썬의 집합자료형 set를 사용한다

---

### **set의 특징**

- 중복을 허용하지 않는다 → 교집합, 차집합, 합집합 구할때 유용
- 순서가 없다 → 따라서, 인덱싱으로 접근하려면 리스트나 튜플로 변환

---

```python
class Solution:
    def hasDuplicate(self, nums: List[int]) -> bool:
        
```

에서 self는 def hasDuplicate 함수가 적용될 인스턴스 객체

(Solution 클래스로 생성한 인스턴스에 hasDuplicate를 적용하고

그 적용될 대상이 인스턴스 자기 자신이라는 뜻의 self)

매개변수 nums는  정수형의 리스트 List[int] 를 받는다.

→ bool 은 def의 리턴값이 True or False 임을 의미

---

### **set을 적용하면 중복 제외한 값만 출력이 됨**

~ 그럼 중복이 있는 리스트는 원래의 원소 개수와 set 적용 후의 원소 개수가 다를 것

~ len 적용해서 원소 개수가 다르면 True, 아니면 False 반환하도록

### 최종 코드

```jsx
class Solution:
    def hasDuplicate(self, nums: List[int]) -> bool:
        if (len(set(nums)) != len(nums)) :
            return True
        else :
            return False
```

⇒ O(n), O(n)
