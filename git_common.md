# 常用git命令

### git最基础的工作流程：分支-开发-推送-合并
![image](Git/git工作流.jpg)
```
//创建新的分支，并修改
git checkout -b feature //创建名为feature的分支，并切换到新的分支
git add newfile.md //增加一个新的文件
git commit -m "my comment"  //添加注释

//推送本地分支到远端
git push    

//合并分支到master主线
git checkout master     // 首先切换到master主线
git merge feature       //合并feature分支到master
```

### git工作流的三个部分：工作区-暂存区-远端
![image](Git/git工作流区域.jpg)
```
//工作区就是你写代码的地方
//暂存区是暂存代码变更的地方
//远端是存放公共项目文件的服务器

//Git能识别你在工作区对代码所做的更改，并能通过add命令放到暂存区，暂存区的文件通过push提交到远端。注意：任何在工作区或者暂存区的东西，只要你不推送的远端，别人是看不见的。

//另外，我们可以通过pull命令将远端的代码拉去（下载）到本地
git pull
```
