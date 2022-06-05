|제목|내용|설명|
|---|---|---|
|top명령어 역할|실시간으로 CPU사용률을 체크해주는 명령어, 디바이스의 성능이나 리눅스 서버의 성능 체크할 때 많이 사용됨. top명령어의 위쪽은 시스템의 상태, 아래는 실행되고 있는 프로세스의 현황이다.|![화면 캡처 2022-06-05 000711](https://user-images.githubusercontent.com/106869861/172036072-c9922b5a-107d-461f-9c8a-d597501a7b64.png)|
|top옵션|shift + p|CPU 사용률이 높은 프로세스 순서대로 표시 ![화면 캡처 2022-06-05 100806](https://user-images.githubusercontent.com/106869861/172036164-3c8cc5bf-6d24-4031-951b-f4ea62539750.png)|
|top옵션|shift + m|메모리 사용률이 높은 프로세스 순서대로 표시![화면 캡처 2022-06-05 100846](https://user-images.githubusercontent.com/106869861/172036203-c1473bc5-a814-4890-8ea1-31537e4639c1.png)|
|top옵션|shift + t|프로세스가 돌아가고 있는 시간 순서대로 표시![화면 캡처 2022-06-05 100926](https://user-images.githubusercontent.com/106869861/172036227-319f41b5-6245-4452-8cf7-c17021c0894e.png)|
|top옵션|Page UP, Page Down|UP : 프로세스의 이전페이지 목록![화면 캡처 2022-06-05 101043](https://user-images.githubusercontent.com/106869861/172036344-8417c733-67b5-4e7e-b673-2754976326c6.png) Down : 프로세스의 다음페이지 목록![화면 캡처 2022-06-05 101008](https://user-images.githubusercontent.com/106869861/172036355-a76a65d7-96f4-43ce-a809-45e02acf4d38.png)|


|제목|내용|설명|
|---|---|---|
|ps명령어 설명|ps명령어는 process status의 줄임말인데, 이 명령어는 실행중인 프로세스 목록과 상태를 보여준다.|![화면 캡처 2022-06-05 101419](https://user-images.githubusercontent.com/106869861/172036395-eed9a452-b5e6-4d2d-8d7f-a2ab4dccddc8.png)|
|ps옵션|-e|모든 프로세스를 출력![화면 캡처 2022-06-05 101438](https://user-images.githubusercontent.com/106869861/172036406-bef36265-f6f3-400e-9b75-ceb4c0516bca.png)|
|ps옵션|-f|완전한 포멧![화면 캡처 2022-06-05 101543](https://user-images.githubusercontent.com/106869861/172036414-382c0e15-0b17-462c-a937-25f9ebce93ce.png)|
|ps옵션|-l|긴 포멧![화면 캡처 2022-06-05 101520](https://user-images.githubusercontent.com/106869861/172036417-7fc17e19-1c1e-4f63-ba9b-b70113b25c05.png)|
|ps옵션|-ef|모든 프로세스를 풀 포멧![화면 캡처 2022-06-05 101708](https://user-images.githubusercontent.com/106869861/172036526-23502eee-ea18-4b4d-a2f0-43673f91025f.png)|
|ps옵션|ps -efㅣgrep '프로세서'|해당 프로세스의 구동을 확인|
|ps추가옵션|a, u, x, f, ww| a - 모든 사용자, u - 프로세스의 사용자, x - 데몬 프로세스, f - 프로세스 상속관계 트리구조로 출력, ww - 넓게|


|제목|내용|설명|
|---|---|---|
|jobs명령어|작업의 상태를 표시하는 명령어로, 쉘 세션에서 실행한 백그라운드 작업의 목록이 출력됨, jobs명령어는 jobs [옵션][작업번호] 형태로 입력하며, 번호는 각 작업의 번호들을 의미하며, 옵션은 -l, -n, -p가 있다|![화면 캡처 2022-06-05 105610](https://user-images.githubusercontent.com/106869861/172036668-132ab612-4377-4877-94e3-1f88f5610178.png)|
|jobs옵션|-l, -n, -p|-l : 프로세스 그룹 ID를 state 필드 앞에 출력, -n : 프로세스 그룹 중에 대표 프로세스 출력, -p : 각 프로세스 ID에 대해 한 행씩 출력 추가로 command옵션은 지정 명령어를 실행합니다.|

+) jobs명령어를 시행해도 시행값이 나오지 않아 스크린샷을 미첨부 했습니다.


|제목|내용|설명|
|---|---|---|
|kill명령어|kill에 대한 설명|대부분 프로세스를 죽이는 것에 사용하는데, 하지만 프로세스에 시그널을 보내 원하는 작업을 하게 하는 명령어이다.kill명령어는 kill [옵션]<pid>로 입력하며 또는 kill [pid]로 입력하면, 프로세스를 죽일 수 있습니다.|
|kill|kill [pid]|![화면 캡처 2022-06-05 110234](https://user-images.githubusercontent.com/106869861/172036854-2743c31f-1d8c-4759-9411-b2c918bf1df1.png) ![화면 캡처 2022-06-05 110247](https://user-images.githubusercontent.com/106869861/172036872-61a9988b-87ba-4633-a8ac-64a9e874e616.png)|
|kill시그널|kill -s [signal][pid]| 시그널 전송방법은 kill -s [signal] [pid]로 입력하며, 여기서 -s 명령으로 다른 시그널을 보냅니다. 그리고, signal의 종류는 kill -l을 이용하여 그 목록들을 확인 할 수 있다.|
|kill|kill -l|시그널 목록 ![화면 캡처 2022-06-05 110432](https://user-images.githubusercontent.com/106869861/172036915-d7c2b6aa-64e9-477f-9520-96e5132e2730.png)|


|제목|내용|설명|
|---|---|---|
