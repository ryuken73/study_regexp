# [10일차] Characters optional
[optional character] <https://regexone.com/lesson/optional_characters>

## kleene's star처럼 하나의 문자에 대해서도 optional을 표현할 수 있다.
 1. ? 메타문자를 통해 optional character를 표현할 수 있다.
 2. ab?c 는 abc도 매칭되고 ac도 매칭된다. 즉 b가 optional이다.
 3. ab*c 도 가능하지만 이건 abbbc도 매칭되어서, 범위가 넓다.
 4. 또는 ab{0,1}c도 되기는 할 것 같다.

## 연습문제
### 아래를 만족시키시오
```
match 1 file found?
match 2 files found?
match 24 files found?
skip No file found
```

`\d+ files? found\?`가 답이다.

* 숫자는 얼마나 클지 모르니 \d\d?가 아니라 \d+가 맞다.   
* files?는 적절하다. file 또는 files니까
* 마지막 found\?는 meta문자를 적절하게 escape처리해야 한다는 걸 보여준다.  
