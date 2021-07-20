# [7일차] Character Ranges
[Character Ranges] <https://regexone.com/lesson/character_ranges>

## [ ]안의 문자들이 순차적이라면(sequential charaters) 
 1. []안에 그 문자들을 다 쓰면 되지만, 이보다 좋은 방법을 고민했을 것 같다. (예: `[abcdefg]`, `[^123456790]`)
 2. 그래서 만들어진것이 [-], 즉 sqaure bracket안의 `-` 대쉬문자이다.  
 3. `-`를 중심으로 그 안에 들어오는 character들을 모두 표현하게 된다.
 4. `-`가 여러번 와도 된다. 즉 `[a-zA-Z0-9]`는 모든 영문 Text와 매칭된다.
 5. 모든 영문자는 metacharacter `\w`로도 표현된다. (반대는 `\W`이다.) 

## 연습문제
### 아래를 만족시키시오
```
match Ana
match Bob
match Cpc
Skip aax
Skip bby
skip ccz   
```

`[A-C]..`가 답이 될수 있다.   
`[^a-c][n-p][a-c]` 도 된다.
