### 封装了 wx.request 的 方法

- get
- post

### 例子

- 先安装

```
npm i wx-api-common
```

- 使用小程序构建 npm

- 全局配置文件 index.js 的写法，之后每个文件引用该文件即可

```
import api from 'wx-api-common';

export default api.setOption({
  baseUrl: '', //  接口的基础地址配置
  params: {
    //  基础参数，即每次调用都要传的参
    access_token: 'access_token',
  },
  request: (a) => { //  请求拦截器
  },
  response: (res) => {  //  回调拦截器
  },
});
```
