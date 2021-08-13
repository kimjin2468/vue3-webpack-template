# Vue3 템플릿 with Webpack

# Packages
webpack: 모듈(패키지) 번들러의 핵심 패키지    
webpack-cli: 터미널에서 Webpack 명령(CLI)을 사용할 수 있음  
webpack-dev-server: 개발용으로 Live Server를 실행(HMR)  

html-webpack-plugin: 최초 실행될 HTML 파일(템플릿)을 연결  
copy-webpack-plugin: 정적 파일(파비콘, 이미지 등)을 제품(dist) 폴더로 복사  

sass-loader: SCSS(Sass) 파일을 로드  
postcss-loader: PostCSS(Autoprefixer)로 스타일 파일을 처리  
css-loader: CSS 파일을 로드  
style-loader: 로드된 스타일(CSS)을 \<style>로 \<head>에 삽입  
babel-loader: JS 파일을 로드  
vue-loader: Vue 파일을 로드  
vue-style-loader: Vue 파일의 로드된 스타일(CSS)을 \<style>로 \<head>에 삽입  
file-loader: 지정된 파일(이미지)을 로드  
  
@babel/core: ES6 이상의 코드를 ES5 이하 버전으로 변환  
@babel/preset-env: Babel 지원 스펙을 지정  
@babel/plugin-transform-runtime: Async/Await 문법 지원  

sass: SCSS(Sass) 문법을 해석(스타일 전처리기)  
postcss: Autoprefixer 등의 다양한 스타일 후처리기 패키지  
autoprefixer: 스타일에 자동으로 공급 업체 접두사(Vendor prefix)를 적용하는 PostCSS의   플러그인    

vue: Vue.js 프레임워크  
@vue/compiler-sfc: .vue 파일(SFC, 3버전)을 해석  

eslint: 정적 코드 분석 도구 (+ESLint)  
eslint-plugin-vue: Vue.js 코드 분석 (+ESLint)  
babel-eslint: ES6 이상의 코드(Babel)를 분석 (+ESLint)  

vuex: 중앙 집중식 저장소 (+Vuex)  
vue-router: 라우터 (+VueRouter)  

# 주의 사항!
 - npm i vue@next 로 설치 (3버전)
 - npm i vue-loader@next 로 설치 (3버전)
 - npm i -D @vue/test-utils@next 로 설치(3버전)
 - npm i -D vue-jest@next로 설치 (3버전)
 - npm i -D webpack-dev-server@next로 설치 (webpack-cli버전(@4^)과 일치)!
 - package.json 옵션으로 browserslist 추가!
 - .postcssrc.js 생성(PostCSS 구성 옵션)!
 - .babelrc.js 생성(Babel 구성 옵션)!
 - .eslintrc.js 생성(ESLint 구성 옵션)! (+ESLint)

 # ESLint Auto fix on save for VSCode 옵션
 - 모든 명령 표시(Windows: Ctrl + Shift + P / macOS: cmd + Shift + P)
 - 모든 명령 표시에서 settings 검색
 - Preferences: Open Settings (JSON) 선택
 - 오픈된 settings.json 파일에서 아래 코드 추가 및 저장

```js
{
  "editor.codeActionOnSave": {
    "source.fixAll.eslint":true
  }
}
