## React MaterialUI활용 로그인 페이지 만들기

<br/>

> Youtube 영상 참고해서 로그인 페이지 만들어보기.

<br/>

[참고소스](https://github.com/mui/material-ui/blob/v5.10.0/docs/data/material/getting-started/templates/sign-in/SignIn.tsx "REACT MUI SOURCE CODE") <b>REACT MUI SOURCE CODE</b>

[참고영상](https://www.youtube.com/watch?v=PWePBteFeeE "생활코딩-React MUI (Material UI)로 로그인 UI 만들어보기") <b>생활코딩-React MUI (Material UI)로 로그인 UI 만들어보기</b>

<br/>

### Let's Go

1. React 프로젝트 만들기
   - npx react-create-app 프로젝트명
2. React UI 라이브러리 - MaterialUI
   - [MUI](https://mui.com/) <b>MUI</b>
     - npm install @mui/material @emotion/react @emotion/styled
   - MUI-icons 사용
     - npm install @material-ui/icons

<br/>

### Search

컨테이너 사이즈 알아보기 -> keywork : mui-breakpoints

### Issues

1. MUI-icons 사용하려고 패키지 다운로드시 npm 에러발생

```javascript
npm ERR! While resolving: pug-loader@2.4.0
npm ERR! Found: pug@3.0.2
npm ERR! node_modules/pug
npm ERR!   dev pug@"^3.0.2" from the root project
npm ERR!   peer pug@"^2.0.0 || ^3.0.0" from pug-plain-loader@1.1.0
npm ERR!   node_modules/pug-plain-loader
npm ERR!     dev pug-plain-loader@"^1.1.0" from the root project
npm ERR!
npm ERR! Could not resolve dependency:
npm ERR! peer pug@"^2.0.0" from pug-loader@2.4.0
npm ERR! node_modules/pug-loader
npm ERR!   dev pug-loader@"^2.4.0" from the root project
npm ERR!
npm ERR! Conflicting peer dependency: pug@2.0.4
npm ERR! node_modules/pug
npm ERR!   peer pug@"^2.0.0" from pug-loader@2.4.0
npm ERR!   node_modules/pug-loader
npm ERR!     dev pug-loader@"^2.4.0" from the root project
npm ERR!
npm ERR! Fix the upstream dependency conflict, or retry
npm ERR! this command with --force, or --legacy-peer-deps
npm ERR! to accept an incorrect (and potentially broken) dependency resolution.
```

> npm 7버전 이 후 dependency conflict 이슈 생김

<br/>

--force: bypass the conflict<br/>
--legacy-peer-deps: ignore peer dependencies entirely

<br/>

[참고글](https://velog.io/@yonyas/Fix-the-upstream-dependency-conflict-installing-NPM-packages-%EC%97%90%EB%9F%AC-%ED%95%B4%EA%B2%B0%EA%B8%B0) <b>npm install '--force' and '--legacy-peer-deps'</b>
