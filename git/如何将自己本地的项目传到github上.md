只需要命令就可以把本地的项目上传到自己的github上。。步骤如下：

1.登陆自己的github账号，如下图所示：

![](https://img-blog.csdn.net/20170810151659042?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc2h1NTgwMjMx/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)

2.点击new repository进行创建一个新的仓库，用来存放自己的项目;

![](https://img-blog.csdn.net/20170810152002947?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc2h1NTgwMjMx/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)

3.也是最重要的部分，用命令将项目上传；

1.cd 到上传项目的根目录下，然后初始化本地仓库，

git init

2.添加当前工作目录文件到index，添加管理，

git add .(记得有个点哦，并且和add之间有空格)

3.查看一下当前目录所有没有被git管理的文件以及被git管理并且被修改但是还没有提交的文件，

git status       （若出现了很多红色文件，那么就需要再次进行2的步骤，git add .直到没有问题。）

4.提交文件，把本地仓库暂存区的文件提交到本地仓库。

git commit -m "message"       其中message就是你提交文件时候的备注。以便知道本次提交是什么作用……

5.关联远程仓库，其中origin后跟的是，远程仓库的别名。

git remote add origin https://github.com/bendan321/nihao.git

6.push文件。


git push -u origin master。



OK，这样的话，就完成了将本地项目传到github上了。

![](https://img-blog.csdn.net/20170810153919421?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc2h1NTgwMjMx/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)