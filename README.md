- 👋 Hi, I’m @d10S3
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
d10S3/d10S3 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

// Android Studio Certificate setting
- 스튜디오 인증서 등록 : 
  Android Studio Preferences -> Tools -> Server Certificates -> Accepted certificates에서 (+)을 클릭 이전에 저장한 인증서를 검색한 다음 Apply
  
- 인증 갱신 경로 확인 : 
  File -> Project Structure JDK location 확인 후
  터미널에서 JDK location 이동

- 인증 갱신 시작 :
  ./bin/keytool -importcert -file /my/certificate/path/my.cer -keystore ./lib/security/cacerts -storepass changeit -noprompt

- File -> Invalidate Caches / Restart
  

// git 주요 커맨드
- git status
- git add *
- git commit -m "commit message" upload
- git push -u origin master

// emulator host 변경

첫번째 터미널

1. /Users/owner(사용자계정)/Library/Android/sdk/emulator 이동
2. ./emulator -avd test(에뮬레이터명) -writable-system

두번째 터미널

1. /Users/owner(사용자계정)/Library/Android/sdk/platform-toos 이동
2. ./adb devices
3. ./adb -s emulator-5554 root
4. ./adb -s emulator-5554 remount
5. ./adb -s emulator-5554 pull /etc/hosts /Users/owner/Desktop/host(호스트 복사할 경로)
6.  /Users/owner/Desktop/host/hosts 파일 수정
7. ./adb -s emulator-554 push  /Users/owner/Desktop/host/hosts /etc/hosts
