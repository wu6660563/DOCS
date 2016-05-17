## GIT

### Git简述

Git是一个管理代码的工具（技术），相关产品有：

+ Github
+ gitlab(自己部署内网)
+ os-china -- [http://git.oschina.net/](http://git.oschina.net/)
+ 码市 -- [https://coding.net/login](https://coding.net/login)
+ [https://bitbucket.org/account/signup/](https://bitbucket.org/account/signup/)

开源的SVN代码托管：
+ 淘宝SVN -- [http://code.taobao.org/](http://code.taobao.org/)


### Git/SVN对比
+ Git是分布式的，SVN是集中式
Git更倾向于分布式开发，因为每一个开发人员的电脑上都有一个Local Repository,所以即使没有网络也一样可以Commit，查看历史版本记录，创建项 目分支等操作，等网络再次连接上Push到Server端。
+ Git把内容按元数据方式存储，而SVN是按文件
因为.git目录是处于你的机器上的一个克隆版的版本库，它拥有中心版本库上所有的东西，例如标签，分支，版本记录等。.git目录的体积大小跟.svn比较，你会发现它们差距很大
+ Git没有一个全局版本号，而SVN有
目前为止这是跟SVN相比Git缺少的最大的一个特征。
+ Git的内容的完整性要优于SVN
GIT的内容存储使用的是SHA-1哈希算法。这能确保代码内容的完整性，确保在遇到磁盘故障和网络问题时降低对版本库的破坏。
+ 分支（Branch）在SVN，分支是一个完整的目录，在Git里面是一个指针

### GIT版本
| 版本 | 优势 | 缺点
|--------- |------| ------|
|Github|开源，里面项目多，最大的系统Linux也是在此管理|私有化需要收费，不适合商业用，服务器放在国外，速度慢|
|gitlab|可以构建内网私有专用|若需要在家里也能提交代码，需要隐射公网IP|
|os-china|开源，可以构建私有库，只允许公司内部人员使用，较多公司采用，资产安全问题不需太大担心|出现过一两次宕机现象，不稳定|
|码市 | 开源，可以私有化 | 小公司产品，稳定性未知，适合短期项目尝试，不建议可持续迭代产品放进去 |

```
综合考虑：
公司内网使用Centos架设gitlab服务器，隐射公网IP，允许外部访问
若公司为了方便考虑，也可考虑采用os-china码云开放平台

```

### Git的使用
后续更新
使用教程：http://www.runoob.com/git/git-basic-operations.html



