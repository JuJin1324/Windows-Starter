# Windows-Starter
Windows에서 웹 개발에 필요한 환경 잡기 및 지식 정리

## Scoop
* Scoop : Windows 전용 패키지(응용 프로그램) 설치 관리자
* 공식 페이지 : [링크](https://scoop.sh/)

### Scoop 설치
* <b>Windows PowerShell</b>에서 작업 
* 설치 명령어 : `> Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')`
* 설치정책 변경 : `> Set-ExecutionPolicy RemoteSigned -scope CurrentUser`
* `> ...실행정책을 변경하시겠습니까? Y`
* 다시 설치 명령어 : `> Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')`

### Scoop 사용법
* 패키지(응용프로그램) 찾기 : `> scoop search [찾을 패키지 명]`
* 패키지 설치 : `> scoop install [패키지 명]`
* 패키지 삭제 : `> scoop uninstall [패키지 명]`
* 버킷(저장소) 추가 : `> scoop bucket add [버킷명]`
* 설치된 패키지 목록보기 : `> scoop list`

### aria2
* aria2 : scoop에서 다중연결(Multi-Connection) 다운로드 지원
* 설치 : `> scoop install aria2`

### Chrome
* 구글의 브라우저 크롬 설치를 위한 버킷(저장소) 추가 : `> scoop bucket add extra`
* 설치 : `>scoop install googlechrome`

### OpenJDK 
* OpenJDK 설치를 위한 버킷(저장소) 추가 : `> scoop bucket add java`
* OpenJDK 8 버전으로 설치 : `> scoop install adopt8-hotspot`

### JetBrain 
* 설치 : `> scoop install jetbrains-toolbox`

### Docker
* Docker 실행을 위한 Hyper-V 활성화 
  - 관리자 모드로 PowerShell 실행
  - 다음 명령어 실행 : `> Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All`
  - 윈도우즈 재시작
* 설치 : `> scoop install docker`

### Visual Studio Code
* 설치 : `> scoop install vscode`

### Git
* 설명 : 버전 관리
* 설치 : `> scoop install git`

### GitHub Desktop 
* 설명 : 앱으로 Github 관리 
* 설치 : `> scoop install github`

### Slack
* 설명 : 사내 메신져
* 설치 : `scoop install slack`

### ADB
* 설명 : android platform tools
* 설치 : `scoop install adb`

### tomcat
* 설치 : `scoop install tomcat`

### telnet
* 설치 : `scoop install telnet`

### KaKaoTalk
* 설치 : `scoop install kakaotalk`
