# [9일차] Mr. Kleene, Mr. Kleene
[matching 0 or 1 more characters] <https://regexone.com/lesson/kleene_operators>

## kleene라는 수학자가 얘기한 kleene's star와 kleene's plus가 있다.
## star(*)는 0 또는 그이상의 반복, plus(+)는 1 또는 그 이상의 반복이다.
 1. 반복되는 문자에 대해서 {}를 쓸 수 있다는 것을 배웠다.
 2. {}로 반복 횟수의 최소,최대는 표현가능했지만, 정해지지 않은 반복횟수를 표현할 수는 없다.   
 3. .+, .*, \d+, \d*, [ab]*, [ab]+등 강력한 표현이 가능하다.  

## 연습문제
### 아래를 만족시키시오
```
match aaabcc
match aabbbbc
match aacc
skip a
```

`aa+b*c+`가 답이 될수 있다.  
또는 반복을 표시하는 {}로 표현할 수 있다.
`a{2,3}b{0,4}c{1,2}`