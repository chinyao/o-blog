# 如何在 github 上发起 pull request

相信很多使用了无数次github的小伙伴，在第一次clone别人代码的时候一定会有疑惑：**我要怎么参与 github 上的开源项目？**
所以，参与开源项目的第一步就是需要知道如何 pull request。

官方介绍：[About github pull request](https://help.github.com/categories/collaborating-with-issues-and-pull-requests/)

> About pull request
> Pull requests let you tell others about changes you've pushed to a repository on GitHub.

Pull Request(PR) 一般分为两种：
- [creating a pull request](https://help.github.com/articles/creating-a-pull-request/)
从 一个分支(feature) 往 另外一个分支(master) 发起 **Pull Request**
- [creating a pull request from a fork](https://help.github.com/articles/creating-a-pull-request-from-a-fork/)
从 fork的仓库 往 被fork的仓库 发起 **Pull Request**

## creating a pull request

略(PR Welcome)

## creating a pull request from a fork

### 第零步：尝试

如果你刚刚开始使用`git`，那么你一定会尝试：

```bash
$ git clone https://github.com/OuYancey/o-blog.git
$ cd o-blog
$ # change something
$ git add -A .
$ git commit -m "change something"
$ git push origin master
Username for 'https://github.com': <username>
Password for 'https://lsner@github.com': <password>
remote: Permission to OuYancey/o-blog.git denied to <username>.
fatal: unable to access 'https://github.com/OuYancey/o-blog.git/': The requested URL returned error: 403
```

错误：没有足够的权限。这时，你可能就会通过搜索引擎查找到需要 fork 才能发起 PR。

### 第一步：fork

1.1 找到你想要参与的项目仓库（比如此项目），点击右上角的 **fork**， 如图：

![第一步：fork](/images/2017-05-16-01.png)

### 第二步：commit

2.1 回到你自己的仓库列表，找到刚刚 **fork** 的项目；

2.2 重新打开这篇文章，点击右上角的 EDIT；

![第二步：commit](/images/2017-05-16-02.png)

2.3 在这篇文章最后 PR 名单中，添加上你的大名，按照格式：`- @<your username> <time>`

2.4 填写 commit 信息

**注：也可以通过`git clone`你所 fork 的项目进行`commit`，再推送到你自己的仓库**

### 第三步：create PR

3.1 回到你所 **fork** 的项目的 **首页**

3.2 找到如图的 `New pull request` 按钮

![第三步：create PR](/images/2017-05-16-03.png)

3.3 如下图，左边红框内为**被fork的项目**，右边红框内为**你的项目**

![第三步：create PR](/images/2017-05-16-04.png)

3.4 点击绿色按钮 `Create pull request` 就完成了你这次的 PR

## 注意事项

在参与开源项目之前，一定要注意其 `Contribution guide`。例如：
- [element contributing guide](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.zh-CN.md)
- [ant-design contributing guide](https://github.com/ant-design/ant-design/blob/master/.github/CONTRIBUTING.md)

仔细看看这些内容，你会注意到一个技术向的关键词: **Rebase**
> In element: **Rebase** before creating a PR to keep commit history clear

> In angt-design: 提交 PR 前请 **rebase**，确保 commit 记录的整洁

## 习题

1. 发起一个 PR ，在下面的 PR Lists 中添加上你的大名，注意提交规范( @<username> <time>)，不符合规范可是不会 merge 的哟。
2. 如何进行 **rebase**, 为什么要进行 rebase 操作，他和 merge 的异同？

## PR Lists

- [@OuYancey](https://github.com/OuYancey/) 2017-05-16 18:38
- [@ChinYao](https://github.com/chinyao/) 2017-05-16 18:50
