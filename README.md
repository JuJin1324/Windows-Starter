# Windows-Starter
> Windows 에서 웹 개발에 필요한 환경 잡기 및 지식 정리

## Winget
### 개요
> Windows11 이후 기본 설치 관리자  
> GUI 애플리케이션 위주로 다운 받는다. zsh 같은 애플리케이션은 지원이 약하기 때문에 zsh 관련 애플리케이션은 choco 로 다운로드 받는다.  

### 모두 업데이트
> 명령어: `winget upgrade --all`

### 패키지 찾기 링크
> [Winstall](https://winstall.app)  

### Chocolatey
> 설치: `winget install --id=Chocolatey.Chocolatey  -e`

### windows terminal
> 설치: `winget install --id=Microsoft.WindowsTerminal  -e`

### Notion
> 설치: `winget install --id=Notion.Notion  -e`

### Chrome
> 설치: `winget install --id=Google.Chrome  -e`

### Git
> 설치 : `winget install --id=Git.Git  -e`

### OpenJDK
> OpenJDK 8 버전으로 설치 : `winget install --id=Amazon.Corretto.8.JDK  -e`  
> OpenJDK 11 버전으로 설치 : `winget install --id=Amazon.Corretto.11.JDK  -e`

### Visual Studio Code
> 설치 : `winget install --id=Microsoft.VisualStudioCode  -e`

### JetBrain Toolbox
> 설치 : `winget install --id=JetBrains.Toolbox  -e`

### KaKaoTalk
> 설치 : `winget install --id=Kakao.KakaoTalk  -e`

### Slack
> 설치 : `winget install --id=SlackTechnologies.Slack  -e`

### Docker
> Docker 실행을 위한 Hyper-V 활성화
> * 관리자 모드로 PowerShell 실행
> * 다음 명령어 실행 : `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All`
> * 윈도우즈 재시작
>
> 설치(관리자 모드로 시작) : `winget install --id=Docker.DockerDesktop  -e`
>
> **설정**
> * General -> Use the WSL 2 based engine 체크
> * Resources -> Enable integration with my default WSL distro 체크, Ubuntu-XX.04 체크

---

## Chocolatey
### 개요
> Chocolatey : Windows 전용 패키지(응용 프로그램) 설치 관리자
> 공식 페이지 : [링크](https://chocolatey.org)

### 모두 업데이트
> 명령어: `choco upgrade all -y`

### 사용법
> 패키지(응용프로그램) 찾기 : `choco search [찾을 패키지 명]`
> 패키지 설치 : `choco install [패키지 명]`
> 패키지 삭제 : `choco uninstall [패키지 명]`
> 설치된 패키지 목록보기 : `choco list`

### 패키지 찾기 링크
> [Find Packages](https://community.chocolatey.org/packages)

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

---

## Windows Dos 명령어 
### 기본 명령어
> * `dir`: ls 명령어  
> * `cls`: clear 명령어  
> * `cd`: cd 명령어  
> * `mkdir [생성할 디렉터리]`: mkdir 명령어  
> * `rmdir [삭제할 디렉터리]`: rm -r 명령어  
> * `del [삭제할 파일명]`: rm 명령어
> * `copy [복사할 파일명] [복사할 위치 경로]`: cp 명령어  
> * `netstat -ano |findstr \[::]\:`: 열린 포트확인 

---

## WSL
### 윈도우 하위시스템 리눅스
> WSL 로 우분투를 실행하기 위해서는 먼저 `Windows 기능 켜기 끄기` 를 열어서 다음 항목을 체크한다.  
> * Linux 용 Windows 하위 시스템
> * 가상 머신 플랫폼
> 
> WSL 설치 명령을 위해서는 관리자 권한의 Powershell 을 연 후 다음 명령어를 실행한다.     
> 명령어: `wsl --install`  
> 
> 우분투 배포판을 검색 후 설치한다.
> * 배포판 검색: `wsl --list --online`
> * 배포판 설치: `wsl --install [배포판 이름]`

---

