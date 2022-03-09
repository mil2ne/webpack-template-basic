## 프로젝트 설정
- `npm init -y`
- `npm i -D webpack webpack-cli webpack-dev-server@next`
- `package.json 파일 수정`

```json
"scripts": {
    "dev": "webpack-dev-server --mode development",
    "build": "webpack --mode production"
  },
```

-` webpack.config.js` 생성
