# 当前版本：0.13 #
  * 更新基版本到 Chromium 13.0.782.107

> [查看历史版本](History.md)

> [安全提示](Security.md)

# FAQ #
  * **如何同步旧版本数据？**其实非常简单，先关闭浏览器，然后把旧版本下面的`UserData`文件夹复制或者剪切到新版本文件夹中即可。以后的版本会加入自动更新功能，就不需要再手工操作了。

# 功能 #
  * 通过浏览器配置菜单启动SSH管理器配置自己的SSH帐号（如下图）。浏览器刚启动时需要几秒钟到半分钟左右连接SSH主机建立隧道，这段时间内无法访问被墙的网站。
> ![http://vforchrome.googlecode.com/svn/trunk/007.png](http://vforchrome.googlecode.com/svn/trunk/007.png)
  * 点击模式切换按钮![http://vforchrome.googlecode.com/svn/trunk/switch_mode.png](http://vforchrome.googlecode.com/svn/trunk/switch_mode.png)可以对当前浏览的域名\*设置或取消\*代理模式。当访问的网站在翻墙列表中时，地址栏右侧会显示![http://vforchrome.googlecode.com/svn/trunk/v.png](http://vforchrome.googlecode.com/svn/trunk/v.png)图标。
    * 目前于[AutoProxy](http://code.google.com/p/autoproxy-gfwlist)收集了大概1500个被墙的网址，并经过了测试，将少数现在已经可以直接浏览的网站从列表中删除。
    * 对需要翻墙的网站才使用代理，墙内的网站直接浏览。
    * 使用开放的PAC文件存储代理规则，高级用户可以直接修改vforchrome.pac创建更复杂的自定义规则。
  * 过滤了CNNIC的证书，避免了潜在的SSL劫持。
  * 地址栏右键菜单添加“用IE打开”，方便查看仅为IE设计的网站。
> ![http://vforchrome.googlecode.com/svn/trunk/open_with_ie.png](http://vforchrome.googlecode.com/svn/trunk/open_with_ie.png)

# 为什么制作这个软件 #
  * 目前\*速度较快\*又比较\*私人化，不容易被封锁\*的翻墙方式，大概主要只有VPN和SSH。VPN通常需要安装专用的软件才能使用，配置也比SSH复杂；SSH则简单一些，只需要用putty或plink或其它的ssh客户端程序建立隧道即可当作代理使用，但是即使简便如此并且教程满天飞的情况下，仍有很多人不知道如何配置SSH隧道，如何让浏览器使用代理，也不知道使用firefox加上AutoProxy实现智能翻墙。本软件希望能将这些配置最简化，使得不懂技术也不爱折腾的用户也能轻松浏览任意网站，把\*稍显复杂的配置问题转化为拥有SSH帐号\*的问题。当然，本软件变的毫无存在意义的那一天的到来，是我最希望看到的。

# 为什么选择Chromium #

  * 使用多进程模型和沙盒技术，极大的提高了浏览器的稳定性和安全性，在目前是IE和Firefox不能比的
  * 开放源代码，可以很方便的进行自己所需的修改
  * 基于webkit内核和v8引擎，带来极快的页面渲染速度
  * 简洁的外观，更大的可视范围