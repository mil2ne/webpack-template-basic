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

```js

// import
const path = require('path')

// export
module.exports = {
  // 파일을 읽어들이기 시작하는 진입점 설정
  entry: './js/main.js',

  // 결과물(번들)을 반환하는 설정
  output: {
    // path: path.resolve(__dirname, 'dist'),
    // filename: 'main.js',
    clean: true // 기존 필요하지 않은 내용 제거
  }
}

```

- `npm run build`

- `npm i -D html-webpack-plugin`
- `npm run dev`
- `npm i -D copy-webpack-plugin`