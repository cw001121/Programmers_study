## 잘라서 배열로 저장하기

### 코드 설명

주어진 `my_str`을 자를 크기인 `n`으로 나눈 수만큼 for문을 돌면서 자른 문자열을 `answer`에 저장

ⅰ) 문자열은 기본적으로 n개씩 잘라서 배열에 넣는다

ⅱ) 마지막 순서에 남은 문자가 n개보다 작더라도 그대로 배열에 넣는다.

### 관련 이슈

1. range 범위 결정

   `len(my_str)/n`값이 정수일 때만 그대로 사용하고, 소수일 경우 올림을 해주어야 함.
   => `math.ceil`을 사용하여 올림
