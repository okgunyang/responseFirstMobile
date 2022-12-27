# ionic + cordova 를 활용한 PWA방식의 모바일 앱 만들기

## cordova 설치
```command
npm install -g @ionic/cli cordova
```

## app 생성하기 
```command
ionic start app1 tabs
```
	-> 선택사항은 모두 기본값(Enter 세 번)

## app 실행하기
```command
cd app1

ionic serve
```

## app 편집하기
```
manifest.json 파일을 index.html이 있는 곳에 작성
service-worker.js 파일을 index.html이 있는 곳에 작성
index.html, manifest.json, service-worker.js 을 /app1/src 디렉토리에 붙여 넣기
```

## app 의 platform 추가하기
```
ionic cordova run android		-> AVD가 구축되어 있는 경우

ionic cordova run ios		-> x-code의 에뮬레이터가 구축되어 있는 경우

npm install -g serve			-> 실행이 되지 않는 경우 서버모듈 설치

npm run build			-> 앱을 빌드하기

ionic capacitor add android		-> 캐패시터를 활용하는 경우 android 추가

ionic capacitor build android

ionic capacitor add ios		-> 캐패시터를 활용하는 경우 ios 추가

ionic capacitor build ios
```
