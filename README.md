1. axios 对于部分机型浏览器有兼容问题

解决办法： cnpm install es6-promise --save-dev
          在axios.min.js开头加上
          require('es6-promise').polyfill();
          
2.new URLSearchParams() 对于部分机型浏览器有兼容问题
解决办法：打包js引入 url-search-params-polyfill 依赖

3.es6 语法兼容
解决办法：打包js引入 babel-polyfill 依赖

