# MissonTwo：认识开发必备工具

## 任务目标：

1. 学习版本管理工具; 
2. 学习使用服务器; 
3. 学习如何将自己的代码放到网上去

## 具体步骤：

- [x] （环境搭建）访问github注册一个帐号（也许需要学习一下如何科学上网）（0.5H）
  - 很早之前就注册过github了：Joined GitHubon August 2, 2016
- [x] （知识学习）查看学习资料——《github——怎样使用Github》（1H） 
  - 参考资料：
    - [怎样使用github:知乎](https://www.zhihu.com/question/20070065)
    - [fork的使用](https://www.cnblogs.com/patchouli/p/6511251.html)
  - 顺便学习了markdown的使用，markdown软件：Typora。[markdown教程](https://blog.csdn.net/zhangruishi/article/details/70768923)
  - 初步完成库的创建，安装GitHub桌面版，克隆库到本地，修改本地文件，并通过github桌面版push到GitHub。
  - GitHub desktop - history - right-hand button - revert this commit 取消提交操作。版本回滚：git命令[教程](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/0013744142037508cf42e51debf49668810645e02887691000)
  - 完成分支创建 - 分支合并 - 分支删除。[分支的作用](https://bbs.csdn.net/topics/390826603)
- [x] （环境搭建）在github上创建一个项目：start a project（0.5H）
- [x] （编程实战）将项目clone到本地（0.5H）
- [x] （编程实战）在本地项目中编写任务代码（0.5H）
- [x] （环境搭建）安装git软件（1H）
- [ ] （知识学习）查看学习资料——《git——Git教程》（0.5H）
  - 参考资料： 

    - [git简明指南](http://rogerdudler.github.io/git-guide/index.zh.html)
    - [git教程](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)

  - git学习

    - class1
      - 1.初始化一个Git仓库，使用`git init`命令。
      - 2.添加文件到Git仓库，分两步：
        - 第一步，使用命令`git add <file>`，注意，可反复多次使用，添加多个文件；git add -A添加所有文件
        - 第二步，使用命令`git commit`，完成。
        - git add -A添加所有文件；git status查看是否还有未提交

    - class2
      - 1.通过git log命令可以获取提交的日志。（--pretty=oneline）
      - 2.$ git reset --hard HEAD^ 回退到上个版本 HEAD^^上上个版本
      - 3.git reset --hard 版本号，可以回退到指定版本，
      - 4.版本号查询git reflog
      - 5.HEAD指向当前版本
    - clsaa3
      - 1.$ ssh-keygen -t rsa -C "youremail@example.com"获取ssh key,在主目录.ssh中
      - 2.添加ssh密匙
        - 登陆GitHub，打开“Account settings”，“SSH Keys”页面
        - 然后点“Add SSH Key”，填上任意Title，
        - 在Key文本框里粘贴`id_rsa.pub`文件内容
      - 3.本地仓库关联远程仓库：
        - git remote add origin git@github.com:michaelliao/learngit.git
        - 把上面的`michaelliao`替换成你自己的GitHub账户名 
      - 4.本地库所有内容推送到远程库
        - $ git push -u origin master
- [ ] （环境搭建）如果是使用webstorm的同学将git可执行文件配置到webstorm配置的版本管理git上，使我们可以通过webstorm可视化直接进行git操作。（0.5H）
- [ ] （编程实战）将本地代码先add到版本管理中，再commit提交，最后push到服务器（1H）
- [ ] （环境搭建）使用云服务器（打开我的学院-我的订单-购物小车，即可购买我院服务器），或者使用其他已购买的其他linux云服务器（0.5H）
- [ ] （环境搭建）如果是windows系统，安装Xshell、secureCRT、Putty等远程连接工具；如果是linux或mac系统则可以直接使用系统自带terminal（1H）
- [ ] （知识学习）了解一点linux的基本命令（1H）
- [ ] （编程实战）使用工具或命令远程连接服务器（0.5H）
- [ ] （知识学习）查看学习资料--《svn——SVN使用教程总结 》（0.5H） 
- [ ] （编码实战）在自己的服务器上，如果有安装svn可以直接使用svn checout的命令，将github上自己创建的项目代码拉到服务器上，如果没有安装请先安装svn。（1H）
- [ ] （编码实战）通过域名访问自己服务器上文件夹中的页面。（0.5H）
- [ ] （编码实战）修改自己的本地文件。（0.5H）
- [ ] （编码实战）push修改后的文件到github。（0.5H）
- [ ] （编码实战）连接服务器，将github上更新的文件更新到服务器svn update。（1H）
- [ ] （环境搭建）有条件的可以申请域名（一年也只需几十而已），使用dnspod绑定域名，并通过域名访问（0.5H）
- [ ] （知识学习）完成任务后查看验收标准，确认任务已完成，如果未完成返回相应步骤（0.5小时）
- [ ] （思考答疑）查看深度思考，学有余力的情况下尝试回答深度思考的问题（1小时）









