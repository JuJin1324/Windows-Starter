# Windows-Starter
Windows 설치 이후 개발에 필요한 도구 설치

## Scoop
* Scoop : 패키지(응용 프로그램) 설치 관리자

### Scoop 설치
* Windows PowerShell 에서 작업 
* `> Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')`
* `> Set-ExecutionPolicy RemoteSigned -scope CurrentUser`
* `> ...실행정책을 변경하시겠습니까? Y`

### 사용법
* 패키지(응용프로그램 찾기) : `> scoop search [찾을 패키지 명]`
* 패키지 설치 : `> scoop install [패키지 명]`
* 패키지 삭제 : `> scoop uninstall [패키지 명]`
* 버킷(저장소) 추가 : `> scoop bucket add [버킷명]`

### aria2
* aria2 : scoop에서 다중연결(Multi-Connection) 다운로드 지원
* aria2 설치 : `> scoop install aria2`

### Chrome
* 구글의 브라우저 크롬 설치를 위한 버킷(저장소) 추가 : `> scoop bucket add extra`
* 크롬 설치 : `>scoop install googlechrome`

### OpenJDK 
* OpenJDK 설치를 위한 버킷(저장소) 추가 : `> scoop bucket add java`
* OpenJDK 8 버전으로 설치 : `> scoop install adopt8-hotspot`

### JetBrain 
* JetBrain ToolBox 설치 : `> scoop install jetbrains-toolbox`

### Docker
* Docker 실행을 위한 Hyper-V 활성화 
  - 관리자 모드로 PowerShell 실행
  - 다음 명령어 실행 : `> Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All`
  - 윈도우즈 재시작
* Docker 설치 : `> scoop install docker`

### Visual Studio Code
* Visual Studio Code 설치 : `> scoop install vscode`

### GitHub Desktop 
* GitHub Desktop 설치 : `> scoop install github`

### Slack
* Slack 설치 : `scoop install slack`

### ADB
* android platform tools
* 설치 : `scoop install adb`

### tomcat
* 설치 : `scoop install tomcat`
