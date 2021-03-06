# 3. 우분투 기본 명령어

## 3-1 터미널 창 활성화

### 터미널 창

- 명령 기반 인터페이스 (CLI) 바탕으로 개발된 프로그램
- 터미널 창 활성해 명령을 사용





## 3-2 시스템 날짜와 시각

### 운영체제의 시각

- RTC - Real Time Clock
  - 하드웨어 시계
  - 마더보드/메인보드에서 배터리 전력으로 구동
  - 운영체제의 간섭을 안 받음
- System Clock
  - 소프트웨어 시계
  - 커널에 의해 관리



### 시간 출력

- 현재 시각, 날짜 출력 : `date`
  - 우분투 시스템에서 설정돼 있는 현재 시각과 날짜 출력

- 시간 동기화 : `timedatectl`
  - 하드웨어 시계, 소프트웨어 시계, UTC, 타임존, 시간 동기화 등 출력



### 달력 출력

- 오늘 날짜가 속한 달 출력 : `cal`

- 달력 출력 : `cal [옵션]`
  - 예) `cal 2023`



### 화면 지우기

- `clear`
  - 터미널 창에서 수행한 모든 명령과 실행결과 삭제





## 3-3 시스템 사용자 정보

### 로그인 네임/ID 확인

- 접속한 사용자의 ID : `users`

  - 시스템에 로그인한 사용자들의 사용자 계정을 출력

- 사용 중인 로그인 네임 : `logname`

  - 최초 로그인한 사용자 계정 출력

  - utmp 파일 참조



### 사용자 계정정보

- 로그인한 모든 사용자 계정 : `who`
  - 시스템에 로그인한 사용자들의 사용자 계정, 터미널, 로그인 시각 등 출력
- 현재 우분투 사용자 확인 : `who am i`
  - `who`에 `am i`인자가 붙은 형태
  - 최초 로그인한 사용자 정보 출력
  - `whoami`보다 많은 정보 출력

- 현재 우분투 사용자 확인 : `whoami`
  - 현재 로그인한 사용자 정보 출력
  - su명령으로 사용자 전환했을 경우, 현재 사용중인 로그인 계정 출력
  - utmp 미참조





