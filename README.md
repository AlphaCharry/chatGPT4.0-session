​
首先要了解 官网的cf和arkose ，官网的cf和arkose为提供防欺诈技术，特别是针对自动化攻击和帐户接管等在线威胁。OpenAI 的 arkose的解决方案来验证用户身份，防止自动化脚本和机器人滥用其服务。为了以确保只有真实用户可以注册账户或请求资源.

先来登录官网的没开通GPT4 的账号查看他们的请求，可以用工具，比如F代理，或者比如抓包工具，这里简单的的用F12浏览器自带的查看：



可以看到官网的GPT 中 cookie对话的所有信息，这里先不管他

登录我们的傀儡网站 http:// chatin.online
![673158642f775d2cd34dfc6fc7239af](https://github.com/AlphaCharry/chatGPT4.0-session/assets/38164385/d2acfc08-07ff-402b-86c9-47d91bc84912)

同样 进入GPT页码 ，这时候我们选择plus账号（3.5也能用）

![f6a45f11b2256c5e235c81ecfa1cc9d](https://github.com/AlphaCharry/chatGPT4.0-session/assets/38164385/1dc50510-1308-45d7-8ade-8d5e0ed3f65b)


同样可以看见 傀儡网站自己保存下来的cookie（有用部分）

，这时候我们用抓包工具获取每次请求的参数



在官网和傀儡网站分别访问，会发现官网返回过来的参数格式是一样的

拿一个工具把数据全部抓到本地。
![c3242ac4cf90390fafc93532ba8a59d](https://github.com/AlphaCharry/chatGPT4.0-session/assets/38164385/ef45fb6c-8af3-410f-9a65-e870b9fb0c1e)


通过解析合并，用抓包工具截取傀儡网站的所有cf信息，然后转发给官网，请求，

比如Fiddler 

在官网界面刷新后，重新发送 此时官网全部会自动转发傀儡网站的账号权限，请求成功！


### 傀儡网站地址 https://chat.chatergpt.top/ 已被修复失效（2024.3.28）（大神重新破解）
### 傀儡网站地址 https://chatin.online/ 可用 （无法访问请翻墙）
​
