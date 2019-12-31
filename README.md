# Windows-Starter
Windows 설치 이후 개발에 필요한 도구 설치

## Scoop
* Scoop : 패키지(응용 프로그램) 설치 관리자

### 설치
* Windows PowerShell 에서 작업 
* > `Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')`
* > `Set-ExecutionPolicy RemoteSigned -scope CurrentUser`
* > ...실행정책을 변경하시겠습니까? `Y`
### aria2 설치
*  aria2 : scoop에서 다중연결(Multi-Connection) 다운로드 지원
* > `scoop install aria2`

### Chrome 설치
* 구글의 브라우저 크롬 설치를 위한 버킷(저장소) 추가 : > `scoop bucket add extra`
* 크롬 설치 : >`scoop install googlechrome`

### OpenJDK 설치
* OpenJDK 설치를 위한 버킷(저장소) 추가 : > `scoop bucket add java`
* OpenJDK 8 버전으로 설치 : > `scoop install adopt8-hotspot`

### JetBrain 
* JetBrain ToolBox 설치 : > `scoop install jetbrains-toolbox`
