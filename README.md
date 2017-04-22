# vue2-multipage-sample

> A Vue2 MultiPage Sample Project

## Project Structure

    vue2-multipage-sample
        |--- build
        |--- config
        |--- dist   构建后的目录结构
            |--- index.html         <---------------|
            |--- cart.html          <------------   |
            |--- user.html          <--------   |   |
            |--- static                     |   |   |
                |--- js                     |   |   |
                    |--- user.[hash].js  ---|   |   |
                    |--- cart.[hash].js  -------|   |
                    |--- index.[hash].js -----------|
                    ...
        |--- src
            |--- assets
            |--- components 公共组建
            |--- pages  多页面文件夹（每个子文件夹都是一个独立的页面，约定：文件夹名称为页面名称）
                |--- index
                    |--- index.html
                    |--- index.js
                    |--- App.vue    root-vue-component
                    |--- components 页面内部的组件
                    |--- routes 如果存在页面路由，在此处配置页面路由配置
                        |--- index.js
                |--- cart
                    |--- cart.html
                    |--- cart.js
                    |--- App.vue
                    |--- components
                    |--- routes
                |--- user
                    |--- user.html
                    |--- user.js
                    |--- App.vue
                    |--- components
                    |--- routes
                ...
        |--- static
        |--- package.json

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
