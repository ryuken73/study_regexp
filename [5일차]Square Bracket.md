# [5일차] Square Bracket 
[Matching specific characters] <https://regexone.com/lesson/matching_characters>

## 문자집합 매칭
 1. Dot이 너무 광범위하게 매칭이 되어서, 몇개의 문자만 매칭되게 하고 싶은 경우가 있을 때 사용
 2. []안의 문자들을 기술하면, 그 중 하나의 문자와 매칭되는지 체크할 수 있다. 
 3. [와 ]는 다 메타문자이다.

## 연습문제
### 아래를 만족시키시오
```
match can
match man   
match fan
skip dan
skip ran
skip pan   
```

`[cmf]an`이 답이 될 수 있겠다.
