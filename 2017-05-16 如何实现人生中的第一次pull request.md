## 关于github 如何发起pull request
相信很多即时使用了无数次github的小伙伴，在第一次clone别人代码的时候一定会有疑惑——
**如果我本地改动了，想要提交呢？**

下面就把我第一次pull request的过程告诉大家

- 第一步
```
git clone https://github.com/OuYancey/o-blog.git
```
这里是我拉代码的第一步，这时我把代码拉到了我的本地

我尝试修改一些东西，然后提交，but 当我 git push的时候，问题来了

```
 ➜  o-blog git:(master) ggp
Username for 'https://github.com': lsner
Password for 'https://lsner@github.com':
remote: Permission to OuYancey/o-blog.git denied to lsner.
fatal: unable to access 'https://github.com/OuYancey/o-blog.git/': The requested URL returned error: 403
```
看到没，我的item给我报出这样的警告，我理解为，它是告诉我，我并没有权限来直接向别人的远程仓库来push代码。

- 第二步

既然这样不行那就直接在自己的远程仓库拉代码，发代码不就行了吗，好主意！！
所以关键问题来了
```
没错就是 git fork
```
多么嗨皮，**fork 的实质就是在原来项目的主分支上新建一个分支，**
而我们自己的远程仓库就相当与这样的一个分支。所以这样一来我们就可以快快乐乐的改动代码啦。

- 第三部

当我们把代码发布到远程仓库之后，这时我们就可以向原项目发送一个**pull request**请求，这一步相当于一次==merge commit==

- 第四步
    

```
等待。。。。可以发个微信给原作者，让他赶紧给你merge一下，这样一来，一次简单的pull request就完成了
```


