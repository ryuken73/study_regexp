# [12일차]Starting and Ending
[Starting and ending] <https://regexone.com/lesson/line_beginning_end>

## 가능한 구체적으로 정규표현식을 작성하는 것이 좋다.
 1. 문장의 처음을 나타내는 ^과 끝을 나타내는 $를 사용하면 잘못된 매칭을 막는데 도움이 된다.
 2. 물론, 부정을 나타내는 []안의 ^과는 의미가 다르다는 것을 기억해야 한다.

## 연습문제
### 아래를 만족시키시오
```
match Mission:successful
skip Last Mission:unsuccessful
skip Next Mission:successful upon capture of target
```

`^Mission:successful$`가 답이다.