# 🫐 yarn berry monorepo 템플릿입니다.

![localhost_3000_](https://user-images.githubusercontent.com/95972251/204802950-d9d01e98-af80-424b-a2c3-aa7b0930d76b.png)

:sparkles: yarn berry monorepo 템플릿입니다. :sparkles:
## 📦 yarn 전역 설치 
- 이미 설치되어 있다면 넘어가셔도 됩니다.

```bash
npm install -g yarn
```

## :tada: 폴더 생성 후, yarn berry 설치 및 설정
- yarn-berry-monorepo 폴더 생성 이후 다음 명령어 실행.

```bash
yarn set version berry
```

## :rocket: yarn berry로 프로젝트 시작
- `yarn -v`를 실행하여 yarn 2.0 이상인지 확인 이후 `yarn init`으로 프로젝트 생성.

- package.json 파일을 다음과 같이 설정.
```js
{
  "name": "monorepo",
  "private": true,
  "workspaces": {
    "packages": [
      "package/*"
    ]
  },
  "packageManager": "yarn@3.0.2"
}
```

## 📂 프로젝트 생성
- 터미널로 package폴더로 이동 후에 CRA나 Vite를 이용하여 생성하는 명령어를 입력한다.

```bash
npx create-react-app [프로젝트 명] 

or

yarn create vite
```

-설치가 완료되었으면 생성 폴더로 이동한 후 `yarn`을 입력하여 패키지를 설치하고 CRA로 설치했을 경우 'yarn start' Vite로 생성했을 시 `yarn dev`를 통해 프로젝트를 실행. 

## ✅ typescript, eslint, prettier 설치
- typescript, eslint, prettier를 추가 설치하려면 다음과 같은 명령어 입력
```bash
yarn add -D typescript prettier eslint

and

yarn dlx @yarnpkg/sdks vscode
```

## 📎 출처
- https://minify.tistory.com/40 를 참고하여 작성하였습니다.
