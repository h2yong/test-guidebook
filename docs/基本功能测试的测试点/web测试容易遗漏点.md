---
title: web测试容易遗漏点
description: web测试容易遗漏点
keywords: [web测试容易遗漏点, web测试容易遗漏地方, web测试容易遗漏测试点, web测试]
---

1. 浏览器的后退按钮  
    > 提交表单一条已经成功提交的记录，back后再提交，看系统会如何处理。检查多次使用back健的情况在有back的地方，back，回到原来的页面，再back，重复几次，看是否会报错。
2. 通过修改URL中的参数，向服务器发起请求，看看会有什么样的结果  
    > 利用一些工具，如http watch，可以记录和捕获向服务器发起的URL请求，然后修改其中的参数向服务器发起请求。该功能点可以和安全测试结合起来。
3. 对表单多次提交  
   > 对提交按钮快速多次点击提交，看看会不会在数据库中形成多条记录。网速或响应快时，这点容易被遗漏，但用户的网络可能慢，很容易多次点击提交。如果前端做了处理，试试捕获在提交时生成的URL，绕过页面，再次对服务器发起请求，会有什么结果。
4. 光标的跳转  
    > 执行操作后，光标是否停留在合适的位置。如邮箱登录，输完用户名回车后，光标应该跳转到密码框内。细节问题，但是影响用户感受。
5. tab键是否功能正确  
    > 和光标的跳转类似，特别是在有输入项时，查看tab键的焦点顺序是否正确。
6. 对全角/半角符号的输入测试  
    > 有输入项时，要考虑全/半角字条的输入，及GBK字符。