# 0.13 #
  * 更新基版本到Chromium 13.0.782.107

# 0.12 #
  * 更新基版本到Chromium 12.0.742.91
  * 优化启动速度

# 0.11a #
  * 更新基版本到Chromium 11.0.696.68

# 0.11 #
  * 更新基版本到Chromium 11.0.696.65

# 0.10a #
  * 更新基版本到Chromium 10.0.648.204

# 0.10 #
  * 更新基版本到Chromium 10.0.648.133
  * 更新plink代码到trunk的9125版本

# 0.09a #
  * 更新基版本到Chromium 9.0.597.107
  * 地址栏右键菜单新增“用IE打开”

# 0.09 #
  * 更新基版本到Chromium 9.0.597.98
  * 改进SSH帐号管理器，增加修改功能，可以方便的修改密码了。

# 0.08b #
  * 因为上一个版本没有完全重新编译，所以出现了一些问题，比如使用桌面通知时崩溃。此版本做了全新的build。

# 0.08a #
  * 更新基版本到Chromium 8.0.552.237
  * 解决在Win7下不能设置默认浏览器的问题

# 0.08 #
  * 升级基版本到Chromium 8.0.552.224

# 0.07c #
  * 升级基版本到Chromium 7.0.517.44
  * 去掉了内置的双击关闭标签的功能，现在Google提供了一个扩展[Chrome Toolbox](https://chrome.google.com/extensions/detail/fjccknnhdnkbanjilpjddjhmkghmachn)可以做这件事。

# 0.07b #
  * 基于Chromium 7.0.517.41
  * 修复vfortunnel.exe对于-N参数被遗漏的问题
  * 修复vfortunnel.exe对于本地public\_ssh.xml配置文件处理错误的问题

# 0.07a #
  * 修复了0.07版本的3个问题：1. 不能放在中文路径下的问题；2. 弹出式窗口的地址栏没有模式切换按钮；3. 因为打包时的一个疏忽，导致在64位系统上不能工作。

# 0.07 #
  * 基于Chromium 6.0.472.63
  * 不再自动寻找免费SSH帐号，因为下载配置文件时的安全问题，而且现在几乎没有免费帐号了。请使用配置程序配置自己的帐号。
  * 一些小调整，比如目录结构，改变配置文件名等等。

# 0.06 #
  * 使用Chromium 5.0.375.125 版本。Google在这个版本解决了一些安全问题。

# 0.05 #
  * 添加了SSH主机配置程序，不再需要用户手动编辑XML文件
  * 改进了vfortunnel.exe，性能和稳定性有所提高

# 0.04 #
  * 将vfortunnel.exe下载配置文件的位置更改为http://vforchrome.googlecode.com/svn/trunk/ssh\_metainfo.xml

# 0.03 #
  * ssh\_metainfo.xml文件配置比较复杂，太过程序员风格，不适合用户使用，因此不再随压缩包提供此文件。vfortunnel.exe会自动下载该配置文件，这样的好处是当一些公开的ssh失效时，可以及时更改。如果用户配置了私有帐号，则vfortunnel.exe不会下载ssh\_metainfo.xml文件。