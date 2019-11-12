## svg-sprite-loader 使用
### 错误代码
```
svg-sprite-loader exception
```

```
#.electron-vue/webpack.renderer.config.js
#添加下面代码
    {
        test: /\.svg$/,
        loader: 'svg-sprite-loader',
        include: [path.join(__dirname, '../src/renderer/icons')],
        options: {
          symbolId: 'icon-[name]'
        }
      },
# 修改下面代码
    {
        test: /\.(png|jpe?g|gif|svg)(\?.*)?$/,
        exclude: [path.join(__dirname, '../src/renderer/icons')],# //添加此代码
        use: {
          loader: 'url-loader',
          query: {
            limit: 10000,
            name: 'imgs/[name]--[folder].[ext]'
          }
        }
      },
```