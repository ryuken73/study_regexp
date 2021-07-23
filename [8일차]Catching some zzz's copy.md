# [8일차] Catching some zzz's
[Character Ranges] <https://regexone.com/lesson/repeating_characters>

## { } curly brace를 사용해서 반복되는 문자를 매칭할 수 있다. 
 1. 그동안 문자들을 매핑하는 방법을 배워왔다. (숫자, 문자, WildCard(.), 여러문자중 하나[], 문자레인지중 하나[-])  
 2. 그런데 반복되는 문자들을 쉽게 표현하는 방법이 필요했다. (예를 들면 aaa, abab, xxxxyy)
 3. Curly Brace로 표현가능 하다. `{}`
 4. 형태는 `a{3}`, `[ab]{3}`이 가능하고, 좀 더 지원하는 경우에는 최소,최대반복도 지정할 수 있다. `a{1,2} : a가 최소 한번, 최대 2번`
 5. 휴대폰 번호 같은거 하기 좋겠다. `\d{3}-\d{4}-\d{3}`

## 연습문제
### 아래를 만족시키시오
```
match wazzzzzup
match wazzzup
skip wazup
```

`waz{3,5}up`가 답이 될수 있다.
