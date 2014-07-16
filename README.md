
到 http://msysgit.github.io/ 下载msysgit并安装

在D:/workfiles/下创建文件夹Git，打开git bash 然后进入到Git所在的文件夹

在Git bash命令界面下执行 git clone https://github.com/sbmgroup/Beginner.git

Clone需要一定时间，等完毕后 执行命令 cd Beginner

现在我们创建一个分支，以你的名字命名，比如zhanglei,命令如下
`git checkout -b zhanglei`

此时，你可以在Beginner文件夹下新建一个文件，里面写上一些文字。

再次回到git bash命令界面里，依次执行以下命令

`git add .`
`git commit -m "information added in readme"`

我们需要将新分支推送到远程代码仓库里,在推送之前需要先一些设置，命令如下:

`git config --global user.email "sbmzhcn@gmail.com"`
`git config --global user.name "sbmzhcn"`

注意，邮箱与名字填写你自己的

然后我们执行以下命令推送我们的更改

`git push origin zhanglei`

上面的命令中 zhanglei应该改为你刚才创建的分支名。如果提示origin不存在，你需要做以下操作：

`git remote add origin https://github.com/sbmgroup/Beginner.git`

执行推送命令

`git push -u origin master`


==其它==

列出每个远程库的简短名字 `git remote -v`

查看分支 `git branch`

查看文件更改 `git status`

