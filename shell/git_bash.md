# git bash

### clone项目

```
git clone git@github.com:calamus0427/my-blog.git
```

### 设置用户名和密码

```
$ git config --global user.name "hanzichi" //给自己起个用户名
$ git config --global user.email  "abc@gmail.com" //填写自己的邮箱
```

### 提交代码
```
git add . // 要add的文件，. 表示添加所有
git commit -m 'add files' // 提交更新
git push origin master  // push到远端master上
```

#### 查看远程分支：
```
$ git branch --all 
//or
$ git branch -r
```

#### 删除远程分支
```
git branch -r -d origin/branch-name  
//或者通过推送空分支的方式删除远程分支
git push origin :branch-name 
```

#### 切换分支
```
$ git checkout branchName
```
