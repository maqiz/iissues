1. axios 对于部分机型浏览器有兼容问题

解决办法： cnpm install es6-promise --save-dev
          在axios.min.js开头加上
          require('es6-promise').polyfill();
          
2.new URLSearchParams() 对于部分机型浏览器有兼容问题
解决办法：打包js引入 url-search-params-polyfill 依赖

3.es6 语法兼容
解决办法：打包js引入 babel-polyfill 依赖

4.在单页面应用中微信配置失败，需要刷新才能成功。（uri与当前页面不一致）
解决办法：利用将wx.config改成方法没在react周期函数componentWillMount中调用。
