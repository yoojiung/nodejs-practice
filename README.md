# Node.js

## npm
전 세계의 개발자들이 만든 다양한 기능(패키지,모듈)들을 관리

## node버전 확인
```
$node --version
```
## npm패키지만들기
```
$npm init -y
```
## nvm 버전 설치
```
$ nvm install 설치버전
```
## nvm 버전확인
```
$ nvm ls
```
## nvm 버전변경
```
$ nvm use 변경할 버전
```
## nvm 버전삭제
```
$ nvm uninstall 버전
```
## nvm단축키 찾기
```
-$ nvm --help
```


## parcel-bundler만들기
```
$ npm install parcel-bundler -D
```

## 설치할 때 -D 차이

-D를 붙히면 `개발용 의존성 패키지`가 설치된다  
없다면 일반 의존성 설치  



## pacel을 이용해서 개발 브라우저 열기

package.json에서 scripts부분에서  
```
"dev":"parcel index.html" 변경 후
$npm run dev
```

## 번들(Bundle)
우리가 프로젝트 개발에 사용한 여러 모듈을 하나로 묶는 작업

## 번들 원하는 버전으로 설치
```
$ npm install lodash@버전명
```

## 코드 난독화
-코드 난독화는 작성된 코드를 읽기 어렵게 만드는 작업  
-빌드된 결과는 브라우저에서 해석하는 용도  
-용량을 축소하고 읽기 어렵게 만드는 등의 최적화를 거치는 것이 좋다


## 유의적 버전(SemVer)
major.minor.patch  
ex)12.14.1  
-major : 기존 버전과 호환되지 않는 새로운 버전  
-minor : 기존 버전과 호환되는 새로운 기능이 추가된 버전  
-patch : 기존 버전과 호환되는 버그 및 오타 등이 수정된 버전  
-^ : major 버전 안에서 가장 최신 버전으로 업데이트 가능표시  
     ^ 기호를 없애면 이 프로젝트는 항상 이 버전을 사용하겠다
