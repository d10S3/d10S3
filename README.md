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
- 인증 갱신 경로 확인
  File -> Project Structure JDK location 확인 후
  터미널에서 JDK location 이동

- 인증 갱신 시작
  ./bin/keytool -importcert -file /my/certificate/path/my.cer -keystore ./lib/security/cacerts -storepass changeit -noprompt

// git 주요 커맨드
- git status
- git add *
- git commit -m "commit message" upload
- git push -u origin master
