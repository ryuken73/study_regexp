# [6일차] Excluding Specific Characters
[Excluding Specific Characters] <https://regexone.com/lesson/excluding_characters>

## 지정된 문자를 제외하고 나머지 매칭
 1. []안에서 ^을 쓰면, 그 뒤에 오는 문자들 외의 모든 문자가 매칭된다.
 2. []안의 문자를 화이트리스트 처럼 쓰고 싶을 때 사용하면 된다.(이거 빼고 나머지 다 매칭)  
 3. ^이 없는 []는 블랙리스트 처럼 동작한다.([]안에 작성된 문자들만 매칭)

## 연습문제
### 아래를 만족시키시오
```
match hog
match dog   
skip bog
```

`[^b]og`가 답이다.
5일차에 배웠던 것으로만 답을 만든다면
`[hd]og`도 답이 될 수 있다.
