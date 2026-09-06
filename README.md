# jotangclub
jotangclub-recruit-2026-git

9月5号  

学习了如何添加远程仓库与从远程仓库克隆文件，并在gitskills中学习了
如何克隆  

添加远程仓库  

git remote add origin git@github.com:用户/仓库.git  

从远程仓库克隆  

git clone git@github.com:用户/仓库.git  

学习了如何创造与合并分支  

创建并切换分支  

git switch -c 分支名  

合并分支  

git merge 分支名  

删除分支  

git branch -D 分支名  

学会了如何解决多人对同一分支修改时冲突的问题  

（因一开始未能正确理解问题，在jotangclub仓库中创立了dev与dev2俩个分支，后来才明白是通过俩个目录对一个分支进行修改）  

9月6日  

学习了如何添加标签并区分标签与分支的区别  

标签是指向某次修改的固定指针，无法对标签进行开发与提交，但更加稳定。  

分支是同一个项目的不同线路，可以直接对分支进行开发修改，还可以通过git merge命令将其并入master或其他分支中。  

学习了Fork与Use this template，并分清楚了俩者的区别  

Fork可以在自己仓库修改后通过pull request提交到原仓库，并由原作者选择是否接收。  

Use this template是创建自己的独立仓库，也就是说Use this template后的仓库与原仓库没有关联，可能部分作者因为不希望代码被脱离原仓库使用，会选择关闭此功能。  

学习了自定义git  
$ git config --global color.ui true/false 显示/不显示颜色（虽然现在默认显示颜色）  
  
忽略特殊文件  

配置别名并用git lg 简化了git log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit命令