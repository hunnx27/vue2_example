# example13 - Vue2.X 설치 및 실행 방법

## 설치순서

### 1. 아래 명령으로 Vue 2.X 프로젝트 생성
```
 vue create exampleCLI
```
 옵션 선택시 아래와 같이 셋팅
   1. ? Please pick a preset: **Manually select features**
   2. ? Check the features needed for your project: **Babel, Router, Vuex, Linter**
   3. ? Choose a version of Vue.js that you want to start the project with **2.x**
   4. ? Use history mode for router? (Requires proper server setup for index fallback in production) **Yes**
   5. ? Pick a linter / formatter config: Basic? Pick additional lint features: **Lint on save**
   6. ? Where do you prefer placing config for Babel, ESLint, etc.? **In dedicated config files**
   7. ? Save this as a preset for future projects? **No**


### 2. 아래 명령으로 서버 기동
```
cd ./exampleCLI
npm run serve
```

### 3. 서버 접속 확인
```
  App running at:
  - Local:   http://localhost:8081/
  - Network: http://192.168.150.171:8081/
```

# example 14 - 뷰라우터
## src/router/index.js
- /* webpackChunkName: "about" */ 레이지 로딩시 해당 주석 앞에 입력 필요(페이지별 로딩, 설정 안할 경우 전체 페이지 선로딩)
- ```<router-link to="/">Home</router-link>``` 로 라우터 링크 이동(빌드시 a 태그로 변경됨)
- ```<router-view/>``` 라우터로 링크시 해당 태그에 연결된 컴포넌트가 로드됨
## viwes/*
- 진입점