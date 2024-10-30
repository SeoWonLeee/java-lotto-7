# java-lotto-precourse

### 1. 로또 구입 금액 입력
- 사용자로부터 로또 구입 금액을 입력받습니다.
- 구입 금액은 1,000원 단위로 입력받습니다.
- 1,000원으로 나누어 떨어지지 않는 경우 IllegalArgumentException을 발생시킵니다.
  - "[ERROR] 잘못된 입력입니다. 1,000원 단위로 입력해주세요."라는 메시지를 출력하며, 로또 구입 금액을 다시 입력받습니다.
    <br/>

### 2. 발행한 로또 수량 및 번호 출력
- 구입 금액에 해당하는 만큼 로또를 발급합니다.
- 로또 번호와 보너스 번호는 1부터 45 사이의 숫자여야 하며, 중복되지 않아야 합니다.
- 당첨 번호 추첨 시, 중복되지 않는 숫자 6개와 보너스 번호 1개를 뽑습니다.
- 로또 번호는 오름차순으로 정렬하여 출력합니다.
  <br/>

### 3. 당첨 번호, 보너스 입력
- 사용자로부터 **당첨 번호**를 입력받습니다.
- 입력된 당첨 번호는 쉼표(,)를 기준으로 구분합니다.
- 입력한 당첨 번호가 1 ~ 45 사이의 숫자가 아닌 경우 IllegalArgumentException을 발생시킵니다.
  - "[ERROR] 당첨 번호는 1부터 45 사이의 숫자여야 합니다."라는 메시지를 출력하며, 당첨 번호를 다시 입력받습니다.
- 1개 미만 또는 6개 초과된 당첨 번호를 입력받은 경우 IllegalArgumentException을 발생시킵니다.
  - "[ERROR] 당첨 번호는 6개여야 합니다."라는 메시지를 출력하며, 당첨 번호를 다시 입력받습니다.
- 숫자 이외의 것이 포함된 경우 IllegalArgumentException을 발생시킵니다.
  - "[ERROR] 당첨 번호에는 숫자(1 ~ 45)만 포함되어야 합니다."라는 메시지를 출력하며, 당첨 번호를 다시 입력받습니다.


- 사용자로부터 당첨 번호와 중복되지 않은 **보너스 번호**를 입력받습니다. 
- 입력한 보너스 번호가 1 ~ 45 사이의 숫자가 아닌 경우 IllegalArgumentException을 발생시킵니다.
  - "[ERROR] 보너스 번호는 1부터 45 사이의 숫자여야 합니다."라는 메시지를 출력하며, 당첨 번호를 다시 입력받습니다.
- 1개 미만 또는 1개 초과된 경우 IllegalArgumentException을 발생시킵니다.
  - "[ERROR] 보너스 번호는 1개여야 합니다."라는 메시지를 출력하며, 다시 입력받습니다.
- 숫자 이외의 것이 포함된 경우 IllegalArgumentException을 발생시킵니다.
  - "[ERROR] 보너스 번호에는 숫자(1 ~ 45)만 포함되어야 합니다."라는 메시지를 출력하며, 보너스 번호를 다시 입력받습니다.
    <br/>

### 4. 당첨 내역 출력
- 사용자가 구매한 로또 번호와 당첨 번호를 비교하여 당첨 내역 및 수익률을 계산합니다.
- 당첨 기준과 금액에 따른 결과를 출력합니다.
  - 1등 : 6개 번호 일치 (2,000,000,000원)
  - 2등 : 5개 번호 + 보너스 번호 일치 (30,000,000원)
  - 3등 : 5개 번호 일치 (1,500,000원)
  - 4등 : 4개 번호 일치 (50,000원)
  - 5등 : 3개 번호 일치 (5,000원)
- 수익률은 소수점 둘째 자리에서 반올림하여 출력합니다.
  <br/>