# chatroom-frontend
An anonymous chatroom UI
匿名聊天室UI， 与聊天室后台js配合使用
---

# 打包步骤
npm install

gulp

(then modify any .js file in /src directory, save changes, and /dist will be created...)

# 使用
获得dist/chat.js后，上传到服务器，下面以nginx目录的assets路径为例
+ 对于网站站长， 可以自定义头部添加`<script src="//ws.tianba.tk/assets/chat.js" async="async" fold></script>`, 刷新网页加载js即可
+ 对于其他网页， F12打开控制台，执行以下代码
    ``` javascript
    var s=document.createElement('script');
    s.src='//ws.tianba.tk/assets/chat.js';
    document.body.append(s);
    ```
# 致谢
+ [icheer/chatroom-frontend](https://github.com/icheer/chatroom-frontend)
