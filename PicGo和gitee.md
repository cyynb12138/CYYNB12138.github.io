<meta name="referrer" content="no-referrer" />

# 使用PicGo和gitee为typora配置一个图床

## 1、下载PicGo ##

> 此下载源来自github，可自行选择其他下载源

步骤一：下载[PicGo](https://github.com/Molunerfinn/PicGo/releases)安装完成后并在此处打开。

![](https://gitee.com/cyynbkls/cyy-de-photo/raw/master/img/202310261906002.png)

步骤二：在插件设置里搜索gitee安装1.1.2版本，安装完成后重新启动PicGo。

![](https://gitee.com/cyynbkls/cyy-de-photo/raw/master/img/202310261907650.png)

如果电脑之前并没有下载node此时会弹出需要先安装**node.js**的提示，而且会自动跳转到下面的[网页](https://link.zhihu.com/?target=https%3A//nodejs.org/en/)直接选择左边下载即可。

![](https://gitee.com/cyynbkls/cyy-de-photo/raw/master/img/202310261912889.png)

此时再进入PicGo即可成功下载gitee插件，安装成功后重启即可。

## 2、创建gitee图床仓库

步骤一：到[gitee官网](https://link.zhihu.com/?target=https%3A//gitee.com/)注册一个账号。

步骤二：登录后，在右上角的+号处，点击**新建仓库**。

![](https://gitee.com/cyynbkls/cyy-de-photo/raw/master/img/202310261920419.png)

按照下图所示，设置仓库信息。

![img](https://pic3.zhimg.com/80/v2-49e9bb6eef976ae7d65f607dc3dcb56a_720w.webp)

> 仓库名称可以自己任取喜欢的名字

点击创建，就成功创建了自己的仓库。

步骤三：**获取token（私人令牌）**

在你的gitee头像处，进入**账号设置**。

![](https://gitee.com/cyynbkls/cyy-de-photo/raw/master/img/202310261927137.png)

如下图，点击左侧的**私人令牌**。

![img](https://pic1.zhimg.com/80/v2-89ea1aad7d0cc7e730d247a29842f51c_720w.webp)

如下图，先取消全选，再勾选**projects**，然后提交。

![img](https://pic4.zhimg.com/80/v2-6ee73259669612db5e40cad076f3e233_720w.webp)

提示要输入gitee账户密码，输入即可。

![img](https://pic3.zhimg.com/80/v2-08740cee0713ca7ac45da1078545ec4a_720w.webp)

**到此便获得了私人令牌**，点击**复制**，并保存好。因为该窗口关闭后，将**无法再查看该私人令牌**。

### **3、在PicGo中配置gitee图床**

步骤一：进入PicGo设置界面，在左边点开图床设置找到gitee。

![](https://gitee.com/cyynbkls/cyy-de-photo/raw/master/img/202310261935899.png)

步骤二：按照下图进行gitee图床的配置。

![](https://gitee.com/cyynbkls/cyy-de-photo/raw/master/img/202310261937193.png)

1. **repo**处填写`gitee账户名/仓库名`。
2. **branch**处填写`master`。
3. **token**处填写上一步获取的`私人令牌`。
4. **path**处填写`img`。
5. 其他的保持默认，不用管。

顺便提一下，`gitee账户名/仓库名`可以在你的gitee仓库的网页地址中复制。

截取http://gitee.com/后面部分即可

![](https://gitee.com/cyynbkls/cyy-de-photo/raw/master/img/202310261940280.png)

填写完毕后，点击**确定**，并**设置为默认图床**。

这样就成功搭建好了自己的图床。
