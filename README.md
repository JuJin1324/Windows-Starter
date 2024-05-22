# Windows-Starter
> Windows 에서 웹 개발에 필요한 환경 잡기 및 지식 정리

## Chocolatey
### 개요
> Chocolatey : Windows 전용 패키지(응용 프로그램) 설치 관리자
> 공식 페이지 : [링크](https://chocolatey.org)

### 설치
> 1. Windows + S 를 누른 후 Windows PowerShell 관리자로 열기   
> 2. 다음 명령어 입력: `Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`
> 설치 링크: [Installing Chocolatey](https://chocolatey.org/install#install-with-cmdexe)

### 사용법
> 패키지(응용프로그램) 찾기 : `choco search [찾을 패키지 명]`
> 패키지 설치 : `choco install [패키지 명]`
> 패키지 삭제 : `choco uninstall [패키지 명]`
> 설치된 패키지 목록보기 : `choco list`

### 패키지 찾기 링크
> [Find Packages](https://community.chocolatey.org/packages)

### windows terminal
> 설치: `choco install microsoft-windows-terminal`

### nodejs
> 설치: `choco install -y nodejs`

### Git
> 설치 : `choco install -y git`

### Chrome
> 설치 : `choco install -y GoogleChrome`

### OpenJDK
> OpenJDK 8 버전으로 설치 : `choco install -y corretto11jdk`  
> OpenJDK 11 버전으로 설치 : `choco install -y corretto8jdk`  

### JetBrain Toolbox
> 설치 : `choco install -y jetbrainstoolbox`

### Visual Studio Code
> 설치 : `choco install -y vscode`

### Slack
> 설치 : `choco install -y slack`

### wget
> 설명 : 웹 서버로부터 컨텐츠 가져오기(주로 압축파일 혹은 프로그램 다운로드 용으로 사용)
> 설치 : `choco install -y Wget`

### ntop
> 설명 : Linux 계열의 htop 혹은 glances 대용 프로그램, CLI로 CPU/RAM 상태 및 프로세스 목록 보는 프로그램
> 설치 : `choco install -y NTop.Portable`

### netcat 
> 설명 : 통신을 리스닝 서버를 netcat 명령어를 통해 간단하게 실행 가능
> 설치 : `choco install -y netcat`
> 사용법  
> 1. 외부 서버에 특정 포트로 접속이 가능한지 확인 : `nc -z [외부 서버 주소] [포트]`
> 2. Listening 서버를 로컬에 띄우기 : `nc -l [포트]`

### ADB
> 설명 : android platform tools
> 설치 : `choco install -y adb`

### tomcat
> tomcat 8.5 : `choco install -y tomcat --version=8.5.12`  
> tomcat 9 : `choco install -y tomcat`  

### telnet
> 설치 : `choco install telnet`

### KaKaoTalk
> 설치 : `choco install kakaotalk`

### Docker
> Docker 실행을 위한 Hyper-V 활성화 
> * 관리자 모드로 PowerShell 실행
> * 다음 명령어 실행 : `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All`
> * 윈도우즈 재시작
> 설치(관리자 모드로 시작) : `choco install docker-desktop`

---

