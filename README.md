- ๐ Hi, Iโm @d10S3
- ๐ Iโm interested in ...
- ๐ฑ Iโm currently learning ...
- ๐๏ธ Iโm looking to collaborate on ...
- ๐ซ How to reach me ...

<!---
d10S3/d10S3 is a โจ special โจ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

// Android Studio Certificate setting
- ์คํ๋์ค ์ธ์ฆ์ ๋ฑ๋ก : 
  Android Studio Preferences -> Tools -> Server Certificates -> Accepted certificates์์ (+)์ ํด๋ฆญ ์ด์ ์ ์ ์ฅํ ์ธ์ฆ์๋ฅผ ๊ฒ์ํ ๋ค์ Apply
  
- ์ธ์ฆ ๊ฐฑ์  ๊ฒฝ๋ก ํ์ธ : 
  File -> Project Structure JDK location ํ์ธ ํ
  ํฐ๋ฏธ๋์์ JDK location ์ด๋

- ์ธ์ฆ ๊ฐฑ์  ์์ :
  ./bin/keytool -importcert -file /my/certificate/path/my.cer -keystore ./lib/security/cacerts -storepass changeit -noprompt

- File -> Invalidate Caches / Restart
  

// git ์ฃผ์ ์ปค๋งจ๋
- git status
- git add *
- git commit -m "commit message" upload
- git push -u origin master

// emulator host ๋ณ๊ฒฝ

์ฒซ๋ฒ์งธ ํฐ๋ฏธ๋

1. /Users/owner(์ฌ์ฉ์๊ณ์ )/Library/Android/sdk/emulator ์ด๋
2. ./emulator -avd test(์๋ฎฌ๋ ์ดํฐ๋ช) -writable-system

๋๋ฒ์งธ ํฐ๋ฏธ๋

1. /Users/owner(์ฌ์ฉ์๊ณ์ )/Library/Android/sdk/platform-toos ์ด๋
2. ./adb devices
3. ./adb -s emulator-5554 root
4. ./adb -s emulator-5554 remount
5. ./adb -s emulator-5554 pull /etc/hosts /Users/owner/Desktop/host(ํธ์คํธ ๋ณต์ฌํ  ๊ฒฝ๋ก)
6.  /Users/owner/Desktop/host/hosts ํ์ผ ์์ 
7. ./adb -s emulator-554 push  /Users/owner/Desktop/host/hosts /etc/hosts
