# 포트폴리오 사이트 만들기 프로젝트

## 02/12 오류 발생본
* npm run dev로 실행 시 404 error가 발생
* 폴더를 프로젝트 환경에 맞게 재구성하니 오류가 지속되어 불러오는 경로를 하나하나 디버깅했어도 안됨

* 이 튜토리얼은 하나의 웹사이트를 여러 가지 프레임워크를 사용하여 만드는 방법에 대해 소개합니다. 

* 웹 개발자들은 종종 다양한 프레임워크를 이용하여 작업하게 됩니다. 

* 이 과정에서 여러 가지 프레임워크들을 어떻게 적용하는지 알아보고,  각 프레임워크들의 장단점을 비교 분석하며 학습하게 됩니다.

1. [vite](https://github.com/webstoryboy/port2023-vite)를 이용하여 사이트를 제작합니다. 
2. [react.js](https://github.com/webstoryboy/port2023-react)를 이용하여 사이트를 제작합니다. 
3. [vue.js](https://github.com/webstoryboy/port2023-vue)를 이용하여 사이트를 제작합니다.
4. [next.js](https://github.com/webstoryboy/port2023-next)를 이용하여 사이트를 제작합니다.

* 이 튜토리얼은 포트폴리오 컨셉의 사이트를 4가지 버전으로 반복하여 만들어 보면서, 프론트앤드 개발의 시발점이 될 수 있는 튜토리얼입니다.

* 자바스크립트 프레임워크를 통해 사이트를 효율적으로 만들어 보는 방법을 익힙니다. 
깊이 배우기 보다는 다양한 방법을 사용하여 흐름과 감각을 익히기 위한 튜토리얼입니다. 

---

## 사용 스택
- vite(https://ko.vitejs.dev/) 를 사용하여 사이트를 번들링하고 관리합니다.
- gsap(https://greensock.com/gsap) 를 이용하여 패럴랙스 효과를 줍니다.
- lenis(https://lenis.studiofreight.com/) 를 이용하여 스므스 효과를 구현합니다.
- netlify(https://www.netlify.com/) 를 통해 사이트를 배포합니다.
- git(https://github.com/) 을 사용하여 파일을 관리합니다.
- HTML, CSS 기반으로 웹사이트의 기본 레이아웃 설계하고, 웹 표준 및 웹 접근성을 준수하여 작업합니다. [ARIA(Accessible Rich Internet Applications)](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles)

---

## 프로젝트 실행
- vite를 설치합니다. `npm create vite@latest`
- gsap를 설치합니다. `npm install gsap`
- lenis를 설치합니다. `npm install @studio-freight/lenis`
- vite를 설치 후 환경 설정을 합니다. `vite.config.js`파일을 만들고 다음과 같이 작성합니다.
```javascript
export default {
    root: "src",
    build: {
    outDir: "../public",
    },
};