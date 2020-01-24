# Github 的 Pull Request 教程

先fork别人的项目到自己的仓库中去
clone到本地进行修改，由于是自己的仓库，所以想怎么改都行
再修改完bug后，push回自己的仓库

第一步：fork项目到自己的仓库中
在项目名称右边有fork键，登陆后点击即可fork仓库。完成后将会跳转到你自己的项目分支。

第二步：打开Git Bash或者命令行，将项目下载到本地
$ git clone https://github.com/taotianli/Virgilio.git
Cloning into 'Virgilio'...
remote: Enumerating objects: 61, done.
remote: Counting objects: 100% (61/61), done.
remote: Compressing objects: 100% (52/52), done.
remote: Total 1784 (delta 27), reused 34 (delta 9), pack-reused 1723
Receiving objects: 100% (1784/1784), 7.15 MiB | 123.00 KiB/s, done.
Resolving deltas: 100% (824/824), done.

你需要将git clone后的网址换成你自己的仓库，在看到done之后就代表这个仓库已经下载到了本地。

第三步：进入本地文件，并进行相应修改，这里以修改README.md作为演示。
$ cd Virgilio/
git add README.md
git commit -m 'Modefied the README.'
复制代码第四步：上传到自己的GitHub仓库，并申请Pull Request
上传代码使用git push origin master命令就可以了，在之后就可以申请PR了。

回到主项目分支上，同时点击Pull Request -> New Pull Request，最后如果原作者觉得这个修改可以被加到项目中去，那么他就会同意合并
注意：在作者合并之前，你可以做多次修改，在申请PR后只要push回自己的仓库，GitHub会自动记录修改并同步。
最后让我们在重复一下步骤，fork->clone->add＆push->PR->merged，你学会了吗？


最后是提交更新
提交代码：

1、在本地修改相应文件（或者文件新旧替换）

2、git add **/**/文件名    （文件修改路径）

（注意路径要写对）

3、git status         ----查看当前本地文件信息

4、 git commit -m "更改信息备注"

5、git push               --------提交代码到当前分支
