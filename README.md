## 记录

1. 修复 sass 错误 ：` "node-sass": "^4.13.1",`
2. 引入 pug：
`npm i -D pug pug-html-loader pug-plain-loader`

```
 chainWebpack: config => {
        config.module.rule('pug')
            .test(/\.pug$/)
            .use('pug-html-loader')
            .loader('pug-html-loader')
            .end()
    }
```