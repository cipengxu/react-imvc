# CHANGELOG

## 2.4.0

- 增加对 `typescript` 的支持
- `util` 模块用 `typescript` 重构

## 2.3.0

- 增加对 `react-hooks` 的支持
  - `useCtrl` 获取当前 controller 的实例
  - `useModel` 获取当前的 global state
  - `useActions` 获取当前的 actions 对象

## 2.2.0

- 优化 `controller.redirect` 
  - 支持在更多生命周期里调用，如 `getInitialState`, `shouldComponentCreate`, `componentWillCreate` 等
  - 使用 `throw` 语句模拟浏览器跳转时中断代码执行的效果

## 2.1.0

- 升级 gulp 套件到 v4.x 版本
- 支持打包出 `server-bundle.js`

```javascript
// imvc.config.js
{
  useServerBundle: true, // 开启 serverBundle 模式
  serverBundleName: 'server.bunlde.js', // 如需修改 serverBundle 的文件名，配置该字段
}
```