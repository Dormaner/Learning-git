# 一、概念解释
1. git，一个版本管理软件，一开始它的开发是为了管理linux的，就像我们用word管理论文，但是用git有一个好处，就是可以无限撤销，恢复到以前的任何版本。
1. Github，基于git的一个网站，可以理解为就是git的网页版本，并且可以多人协作一起写代码！
1. 三个基本概念：提交commit、仓库repository、分支branch
Commit红色的代表以前的，绿色的代表新修改的，白色的代表没有修改。
Branch：所有的分支都会合并到main分支里，以前叫master，因为有“主人”的意思，被一群黑人搞政治正确改成了main。

1. Issue就是一个论坛，可以在里面提这个开源软件有哪些需要改进的地方。里面有两种状态，一种是Open，就是别人提了，但是作者团队还没有搭理；另外一种是Closed，就是回复了。
1. Star：就是收藏夹的功能
2. License：注意这个文件里的协议，里面如果是MIT的，大多都是免费，如果是其他的，可能会收费，商用的话一定要注意！

# 二、学习资源
1. 直接在github网站进行仓库搜索
>找百科大全：awesome xxx

>找案例：xxx sample

>找项目模板（配置好了环境，可以直接拿来用）：xxx starter/xxx boilerplate
找教程：xxx tutorial
2. 网站推荐
>https://github.com/trending/（可以根据筛选条件来搜索GitHub项目）

>https://github.com/521xueweihan/HelloGitHub（就像一个期刊一样，每次都介绍一些有趣的GitHub项目，中文的）

# 三、本地文件上传到Github上
## （一）在本地新建文件夹
## （二）在文件夹里建立.git文件
直接在文件夹里右键点击git bash here：git init，回车后就发现文件里多了个隐藏文件.git，这个时候文件夹就变成仓库了。
## （三）在GitHub上新建文件
## （四）建立本地和远程GitHub的链接
一般新建仓库后，就会有链接，复制下来即可，然后输入如git remote add origin https://github.com/Dormaner/TT.git （如果不挂梯子，可能会联网失败）
## （五）将本地文件push到GitHub：
保存、提交更改后，输入命令git push -u origin main。由于政治正确，本地的主分支名称如果是master，需要改一下。
# 四、将GitHub上的仓库pull到本地再进行更改
## （一）新建本地仓库
1、在github上新建仓库
2、点击“Code”--“Code”--“https"，点击复制地址
3、新建vscode文件后，点击左侧“源代码管理”--“克隆仓库”（也可以在源代码管理的右上角点击“克隆”）后复制地址，并选择一个本地仓库

## （二—）将本地内容推送到github上
1、添加内容后，按下“Ctrl+S”保存文件
2、点击源代码管理，输入更改内容，如“增加了openBIM”，点击提交
3、点击“同步更改”

## （三）打开github，刷新即可。
安装vscode后需要安装两个插件
1、Markdown all in one（Markdown编辑器，但预览功能不太好）
2、Markdown Preview Enhanced（可显示流程图等）

# 四、其他问题
## （一）git clone和download zip  有什么区别？
答：通过git clone下载出来的会多一个隐藏文件夹.git，用大白话说其实就是用git clone下载下来的是一个仓库，是可以有后悔药这个功能的，用download zip下载下来的只是一个单纯的文件夹，没有任何和git相关的功能。
## （二）从工作区到仓库为啥有两个步骤？
![Alt text](images/%E5%9B%BE%E7%89%871.png)
答：因为一个文件可能暂时没有写好，这个时候要是扔进仓库里，会让仓库的提交变得很乱，这个时候我们就可以先用git add的命令将文件放到暂存区，等写好了，在放到仓库里。
