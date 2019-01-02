[TOC]

## 编码之前

### 获取代码

- 访问https://github.com/
- 登录`github`，获取代码仓库地址。(用户名：2451183456@qq.com)
- 打开Git 将代码拉取到本地。

```git bash
//克隆仓库到本地
git clone https://github.com/huangjinbiao/algorithm.git
//切换到开发分支
git checkout develop
```



## 编码之后

### 提交代码到github

注意，别提交了不该提交的代码。

```java
git pull
git add .
git commit "xxxx"
```

## 从无到有

idea新建一个项目，添加了代码之后。可以通过以下方式在`GitHub`创建一个代码库，当然也可以在`GitHub`界面上创建。

![idea-share-project-to-github](..\images\idea-share-project-to-github.png)

如果是在`GitHub`界面上创建，则需要再进行以下`git`命令，方能将本地的库与远端的库对接起来。

```git bash

git init
--没有设置之前，需要设置以下，否则会提示please tell us who you are
git config --global user.name huangjinbiao
git config --global user.email 2451183456@qq.com
--与远端连接起来
git remote add origin https://github.com/huangjinbiao/design-pattern.git
-- 不允许提交空文件 先本地提交，在推掉远程
git add pom.xml
git commit -m "init project"
git push --set-upstream origin master
-- 同理远端创建develop分支为
git push --set-upstream origin develop
```

