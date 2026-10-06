# jotangclub

jotangclub-recruit-2026-git —— 焦糖工作室 2026 招新 · Git 学习记录

## 仓库说明

本仓库用于记录我在招新期间学习 Git 的过程与练习，内容按日期分区。
除最终的 Git 练习成果外，还保留了练习分支冲突时使用的 `env.md`。

## 9月5日：远程仓库、克隆与分支

学习了如何添加远程仓库与从远程仓库克隆文件，并在 gitskills 中学习了如何克隆。

添加远程仓库：

```bash
git remote add origin git@github.com:用户/仓库.git
```

从远程仓库克隆：

```bash
git clone git@github.com:用户/仓库.git
```

学习了如何创建与合并分支。

创建并切换分支：

```bash
git switch -c 分支名
```

合并分支：

```bash
git merge 分支名
```

删除分支：

```bash
git branch -D 分支名
```

学会了如何解决多人对同一分支修改时冲突的问题。

> 因一开始未能正确理解问题，在 jotangclub 仓库中创建了 dev 与 dev2 两个分支，
> 后来才明白是通过两个目录对同一个分支进行修改。

## 9月6日：标签、Fork 与自定义 Git

学习了如何添加标签，并区分标签与分支的区别。

- **标签**：指向某次修改的固定指针，无法对标签进行开发与提交，但更加稳定。
- **分支**：同一个项目的不同线路，可以直接对分支进行开发修改，还可以通过
  `git merge` 命令将其并入 master 或其他分支中。

学习了 Fork 与 Use this template，并分清楚了二者的区别。

- **Fork**：可以在自己仓库修改后通过 pull request 提交到原仓库，并由原作者选择是否接收。
- **Use this template**：创建自己的独立仓库，也就是说 Use this template 后的仓库与原仓库
  没有关联。可能部分作者因为不希望代码被脱离原仓库使用，会选择关闭此功能。

学习了自定义 Git：

```bash
git config --global color.ui true   # 显示颜色（虽然现在默认显示颜色）
git config --global color.ui false  # 不显示颜色
```

学习了忽略特殊文件，以及配置别名 —— 用 `git lg` 简化了下面这串命令：

```bash
git log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
```
