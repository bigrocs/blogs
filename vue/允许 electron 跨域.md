## 允许 electron 跨域
```
  mainWindow = new BrowserWindow({
    height: 563,
    useContentSize: true,
    width: 1000,
    webPreferences: { webSecurity: false } // 允许 electron 跨域
  })
```