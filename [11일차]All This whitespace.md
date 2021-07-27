# [11일차]All This whitespace
[whitespace] <https://regexone.com/lesson/whitespaces>

## 로그파일이나 User input에서 whitespace(공백)을 만나지 않기란 어려운 일이다.
 1. whitespace문자로 `\t` (tab), `\n` (new line), `\r` (carrige return)이 있다.
 2. 이 모든 것과 매칭이 되는 강력한 메타문자가 \s이다. (반대는 \S)
 3. 물론 다른 문자와 동일하게 kleene's +, * 가 적용된다.
 4. `\s`는 사용자 입력을 처리하는데 매우 중요한 역할을 할 것이다.

## 연습문제
### 아래를 만족시키시오
```
match 1.  abc.
match 2.    abc.
match 3.      abc.
skip 4.abc.
```

`\d\.\s+abc\.`가 답이다.