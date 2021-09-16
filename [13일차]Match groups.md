# [13일차]Match groups
[Match groups] <https://regexone.com/lesson/capturing_groups>

## 일치한 패턴에서 정확히 필요한 부분만 가져오고 싶을 수 있다. 
 1. 전화번호, 이메일 정보 등 텍스트 뭉치에서 이 정보들만 뽑아야 하는 경우,
 2. 계정정보도 될 수 있고, 아무튼 필요한 데이터들만 가져와야 후처리가 가능한 경우
 3. ()를 사용하면 된다. * ()는 이렇게 capture할 때와 표현식을 그룹화할 때 사용한다.

## 연습문제
### 아래를 만족시키시오 (.pdf빼고 파일명만 capture)
```
capture file_record_transcript.pdf
capture file_07241999.pdf
skip testfile_fake.pdf.tmp
```

`^(file.+)\.pdf$`가 답이다.