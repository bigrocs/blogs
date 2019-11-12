# Vue Babel6 使用 jsx 问题
## 引用
* [**jsx**](https://github.com/vuejs/jsx)
* [**babel-plugin-transform-vue-jsx**](https://github.com/vuejs/babel-plugin-transform-vue-jsx)
### 安装依赖
```
# yarn
yarn add\
 babel-plugin-syntax-jsx\
 babel-plugin-transform-vue-jsx\
 babel-helper-vue-jsx-merge-props\
 babel-preset-env\
 --dev
```
```
#npm
npm install\
  babel-plugin-syntax-jsx\
  babel-plugin-transform-vue-jsx\
  babel-helper-vue-jsx-merge-props\
  babel-preset-env\
  --save-dev
```
### 修改 .babelrc 
```
{
  "presets": ["env"],
  "plugins": ["transform-vue-jsx"]
}
```