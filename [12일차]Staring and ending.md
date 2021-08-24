# [12일차]Staring and ending
[whitespace] <https://regexone.com/lesson/line_beginning_end>

## 더 명확하게(더 좁게) 패턴을 만드는 것이 더 낫다.(잘못된 패턴매칭을 막는 가장 좋은 방법)
 1. ^와 $를 이용해서 라인의 처음과 끝을 표시할 수 있다.
 2. ^...$를 사용해서, 정확히 패턴과 일치하는 라인을 매칭할 수 있다.
 3. [^...]는 다른 의미이다. (부정패턴)
 
## 연습문제
### 아래를 만족시키시오
```
match Mission: successful
skip  Last Mission: unsuccessful 
skip  Next Mission: successful upon capture of target.
```

`^Mission: successful$`가 답이다.