## SRT 자동예매 매크로

사용자가 원하는 시간, 출발지, 목적지 등을 입력해 자동으로 SRT 표를 예매해주는 프로그램입니다.<br/><br/><br/>

## 사용법

main.py 파일을 열고 밑에서 설명하는 각 변수에 사용자의 정보를 입력하면 됩니다.<br/>

```
member_number = "0000000000" # 회원번호
password= "1234" # 비밀번호
arrival = "수서" # 출발지
departure = "동대구" # 도착지
standard_date = "20230217" # 기준날짜 ex) 20221101
standard_time = "16" # 기준 시간 ex) 00 - 22 // 2의 배수로 입력
from_train_number = 1 # 몇번째 기차부터 조회할지  min = 1, max = 10
to_train_number = 10 # 몇번째 기차까지 조회할지 min = from_train_number, max = 10

```

다음으로 Terminal에 다음과 같은 명령어를 입력하여 selenium 모듈을 설치합니다.

```
pip install selenium
```

이후 프로그램을 실행하면 자동으로 SRT 예매가 시작됩니다.

- 같은 IP로 수많은 요청을 보냈을 때 SRT의 자체 보안툴에서 해당 IP를 차단하는 케이스가 감지되었습니다. 이러한 현상을 방지하기 위해 VPN 사용 환경을 권장합니다.
- 반드시 본인이 사용하는 크롬 버전에 맞는 chromedriver.exe 파일을 사용하여야 합니다.
