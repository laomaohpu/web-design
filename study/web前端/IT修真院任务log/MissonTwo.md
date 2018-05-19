# MissonTwo：认识开发必备工具

## 任务目标：

1. 学习版本管理工具; 
2. 学习使用服务器; 
3. 学习如何将自己的代码放到网上去

## 具体步骤：

- [x] （环境搭建）访问github注册一个帐号（也许需要学习一下如何科学上网）（0.5H）
- [x] 2.（知识学习）查看学习资料——《github——怎样使用Github》（1H） 
- [x] 3.（环境搭建）在github上创建一个项目：start a project（0.5H）
- [x] 4.（编程实战）将项目clone到本地（0.5H）
- [x] 5.（编程实战）在本地项目中编写任务代码（0.5H）
- [x] 6.（环境搭建）安装git软件（1H）
- [x] 7.（知识学习）查看学习资料——《git——Git教程》（0.5H） 
- [x] 8.（环境搭建）如果是使用webstorm的同学将git可执行文件配置到webstorm配置的版本管理git上，使我们可以通过webstorm可视化直接进行git操作。（0.5H）
- [x] 9.（编程实战）将本地代码先add到版本管理中，再commit提交，最后push到服务器（1H）
- [ ] 10.（环境搭建）使用云服务器（打开我的学院-我的订单-购物小车，即可购买我院服务器），或者使用其他已购买的其他linux云服务器（0.5H）
- [ ] 11.（环境搭建）如果是windows系统，安装Xshell、secureCRT、Putty等远程连接工具；如果是linux或mac系统则可以直接使用系统自带terminal（1H）
- [ ] 12.（知识学习）了解一点linux的基本命令（1H）
- [ ] 13.（编程实战）使用工具或命令远程连接服务器（0.5H）
- [ ] 14.（知识学习）查看学习资料--《svn——SVN使用教程总结 》（0.5H） 
- [ ] 15.（编码实战）在自己的服务器上，如果有安装svn可以直接使用svn checout的命令，将github上自己创建的项目代码拉到服务器上，如果没有安装请先安装svn。（1H）
- [x] 16.（编码实战）通过域名访问自己服务器上文件夹中的页面。（0.5H）
- [x] 17.（编码实战）修改自己的本地文件。（0.5H）
- [x] 18.（编码实战）push修改后的文件到github。（0.5H）
- [ ] 19.（编码实战）连接服务器，将github上更新的文件更新到服务器svn update。（1H）
- [x] 20.（环境搭建）有条件的可以申请域名（一年也只需几十而已），使用dnspod绑定域名，并通过域名访问（0.5H）
- [ ] 21.（知识学习）完成任务后查看验收标准，确认任务已完成，如果未完成返回相应步骤（0.5小时）
- [ ] 22.（思考答疑）查看深度思考，学有余力的情况下尝试回答深度思考的问题（1小时）

## 学习笔记

### github

1.很早之前就注册过github了：Joined GitHubon August 2, 2016

2.github学习参考资料：

​	[怎样使用github:知乎](https://www.zhihu.com/question/20070065)

​	[fork的使用](https://www.cnblogs.com/patchouli/p/6511251.html)

3.顺便学习了markdown的使用，markdown软件：Typora。[markdown教程](https://blog.csdn.net/zhangruishi/article/details/70768923)

4.初步完成库的创建，安装GitHub桌面版，克隆库到本地，修改本地文件，并通过github桌面版push到GitHub。

5.GitHub desktop - history - right-hand button - revert this commit 取消提交操作。版本回滚：git命令[教程](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/0013744142037508cf42e51debf49668810645e02887691000)

6.完成分支创建 - 分支合并 - 分支删除。[分支的作用](https://bbs.csdn.net/topics/390826603)

### git学习

####1.参考资料：

​	[git简明指南](http://rogerdudler.github.io/git-guide/index.zh.html)

​	[git教程](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)

#### 2.git笔记

##### class1 创建git本地仓库和添加文件到仓库

- 1.初始化一个Git仓库，使用`git init`命令。

- 2.添加文件到Git仓库，分两步：
  - 第一步，使用命令`git add <file>`，注意，可反复多次使用，添加多个文件；git add -A添加所有文件
  - 第二步，使用命令`git commit`，完成。git add -A添加所有文件；git status查看是否还有未提交

##### class2 git版本回退

- 1.通过git log命令可以获取提交的日志。（--pretty=oneline）

- 2.$ git reset --hard HEAD^ 回退到上个版本 HEAD^^上上个版本

- 3.git reset --hard 版本号，可以回退到指定版本，

- 4.版本号查询git reflog

- 5.HEAD指向当前版本


##### clsaa3 获取ssh密匙关联远程仓库和推送到远程仓库

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
- 5.远程仓库克隆
  - $ git clone git@github.com:michaelliao/gitskills.git
  - 注意把Git库的地址换成你自己的 michaelliao/gitskills
  - Git支持多种协议，包括`https`，但通过`ssh`支持的原生`git`协议速度最快 

##### class4 分支管里

- 1.创建与合并分支

  - `HEAD`严格来说不是指向提交，而是指向`master`，`master`才是指向提交的，所以，`HEAD`指向的就是当前分支。 
  - Git鼓励大量使用分支：
    - 查看分支：git branch
    - 创建分支：git branch <name>
    - 切换分支：git checkout <name>
    - 创建+切换分支：git checkout -b <name>
    - 合并某分支到当前分支：git merge <name>
    - 删除分支：git branch -d <name>

- 2.解决冲突

  - 当Git无法自动合并分支时，就必须首先解决冲突。
  - 解决冲突后，再提交，合并完成。
  - 解决冲突就是把Git合并失败的文件手动编辑为我们希望的内容，再提交。
  - 用`git log --graph`命令可以看到分支合并图。

- 3.分支管里

  - 在实际开发中，我们应该按照几个基本原则进行分支管理：

    首先，`master`分支应该是非常稳定的，也就是仅用来发布新版本，平时不能在上面干活；

    那在哪干活呢？干活都在`dev`分支上，也就是说，`dev`分支是不稳定的，到某个时候，比如1.0版本发布时，再把`dev`分支合并到`master`上，在`master`分支发布1.0版本；

    你和你的小伙伴们每个人都在`dev`分支上干活，每个人都有自己的分支，时不时地往`dev`分支上合并就可以了。

  - 合并分支时，加上`--no-ff`参数就可以用普通模式合并，合并后的历史有分支，能看出来曾经做过合并，而`fast forward`合并就看不出来曾经做过合并。

- 4.Bug分支

  - $ git stash  把工作现场储存起来

  - 修复bug时，我们会通过创建新的bug分支进行修复，然后合并，最后删除；

    当手头工作没有完成时，先把工作现场`git stash`一下，然后去修复bug，修复后，再`git stash pop`，回到工作现场。

- 5.feature分支

  - $ git branch -D feature-vulcan 强行删除
  - 开发一个新feature，最好新建一个分支；如果要丢弃一个没有被合并过的分支，可以通过`git branch -D <name>`强行删除。

- 6.多人协作

  - 查看远程库信息：$ git remote  加 -v显示更详细信息 如果没有权限看不到push地址
  - 推送分支
    - $ git push origin master 推送master分支
    - $ git push origin dev 推送其他分支

- 7.Rebase

  - rebase操作可以把本地未push的分叉提交历史整理成直线；

    rebase的目的是使得我们在查看历史提交的变化时更容易，因为分叉的提交需要三方对比。

##### class5标签管里

- 1.标签管里
  - tag就是一个让人容易记住的有意义的名字，它跟某个commit绑在一起。 
- 2.创建标签
  - 1.切换到需要打标签的分支 $ git branch
  - 2.$ git tag <name> 打上一个新标签 
    - 默认标签是打在最新提交的commit上的 
    - 忘记打标
      - 先找到历史提交的commit id 
      - $ git tag <name> commit id
  - 3.$ git tag查看所有标签 
    - 标签不是按时间顺序列出，而是按字母排序的。 
    - $ git show <tagname> 查看标签信息
  - 4.创建带有说明的标签，
    - 用`-a`指定标签名，`-m`指定说明文字
    - $ git tag -a v0.1 -m "version 0.1 released" 1094adb
    - git show <tagname>可以看到说明文字
- 3.操作标签
  - 1.删除 $ git tag -d <tagname>
  - 2.推送某个标签到远程 git push origin <tagname>
  - 3.一次性推送全部尚未推送到远程的本地标签： $ git push origin --tags
  - 4.删除远程标签
    - 1.删除本地标签 $ git tag -d <tagname>
    - 2.$ git push origin :refs/tags/<tagname>

##### class6使用GItHub

- 1.Fork在自己账号下克隆仓库
- 2.git克隆库到本地
- 3.github发起pullrequst请求希望官方能够接受修改:贡献代码

##### class7使用码云

- 1.国内的Git托管服务——[码云](https://gitee.com/)
- 2.5人以下小团队免费 
- 3.[码云托管](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/00150154460073692d151e784de4d718c67ce836f72c7c4000)
  - git remote add把它和码云的远程库关联
    - git remote add origin git@gitee.com:liaoxuefeng/learngit.git
    - git remote -v查看远程库信息
    - git remote rm 远程库名 可以删除远程库
    - 关联多个库
      - git remote add github git@github.com:michaelliao/learngit.git
        - 远程库的名称叫github，不叫origin了。 
      - git remote add gitee git@gitee.com:liaoxuefeng/learngit.git
        - 同样注意，远程库的名称叫gitee，不叫origin
        - git@github.com:laomaohpu/learngit.git

##### class8自定义Git

1.忽略特殊文件

- 在Git工作区的根目录下创建一个特殊的[gitignore文件](https://github.com/github/gitignore)，然后把要忽略的文件名填进去，Git就会自动忽略这些文件。 
- 忽略文件的原则是：
  - 1.忽略操作系统自动生成的文件，比如缩略图等；
  - 2.忽略编译生成的中间文件、可执行文件等，也就是如果一个文件是通过另一个文件自动生成的，那自动生成的文件就没必要放进版本库，比如Java编译产生的`.class`文件；
  - 3.忽略你自己的带有敏感信息的配置文件，比如存放口令的配置文件。
- $ git add -f App.class被忽略文件强制添加到git
- $ git check-ignore -v App.class 检查规则
- .gitignore文件本身要放到版本库里，并且可以对.gitignore做版本管理！

2.配置别名

- $ git config --global alias.st status 用st表示status
- 配置Git的时候，加上`--global`是针对当前用户起作用的，如果不加，那只针对当前的仓库起作用。 
- 配置文件放哪了？每个仓库的Git配置文件都放在.git/config文件中
-  当前用户的Git配置文件放在用户主目录下的一个隐藏文件.gitconfig中

3.搭建Git服务器

- [详细教程](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/00137583770360579bc4b458f044ce7afed3df579123eca000)

##### class9git补充资源教程

* [gitlog进阶](https://www.cnblogs.com/bellkosmos/p/5923439.html)

#### 3.webstorm配置git













