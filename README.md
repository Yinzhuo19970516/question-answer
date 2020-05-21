# 问答系统的设计与实现
### 预期实现的功能
* 问答系统前端设计和实现，一般用户可以在 此发表提问，专家用户可以进行回答，并获取报酬等;
* 问答系统的后端实现， 包括问答管理，用户管理，支付管理，存储机制等，
* 管理后台实现，管理员 可以在管理后台进行问答系统的管理。
* 分布式爬虫自动获取问题的答案

### 技术方案

* 前端：uni-app(开发完成之后可多端复用，目前只做h5)
* 后端：待定
* 管理后台：vue-admin(待定，先不做)
* 爬虫：Scrapy(待定)

### 主要功能模块
##### 登录注册功能
* 登录，支持社交账号登录（gihtub,微信，qq）
* 注册

##### 首页静态数据的展示

* 轮播图的展示
* 排行榜的展示，点击相应的问题，进入问题详情，可以查看问题的
##### 提问模块

* 表单提交，提交问题，提交项有问题，分类，悬赏积分，多少人回答。
##### 回答问题模块
* 点击进入问题，可以进入问题详情进行回答，并可以修改，删除。
##### 积分模块
* 每个新用户注册都可以获得200积分，提问会消耗积分，回答问题被采纳可以获得积分。
##### 个人中心模块
* 用户可以修改自己个的头像
* 查看自己回答过的问题
* 查看修改删除自己提问的问题
##### 问题搜索模块
* 简单的检索功能


### 一期准备实现功能
- [ ] 登录
- [ ] 上传头像功能
- [ ] 提问功能
- [ ] 回答问题功能

#### 目测需要提供的接口
登录接口
上传头像接口
提交问题接口
获取问题详情接口
回答问题写答案提交接口

### 如何提交自己的改
##### 第一次

1.克隆仓库
> git clone git@github.com:Yinzhuo19970516/question-answer.git

2.切到这个文件
> cd question-answer

3.新建本地分支并切到这个分支
> git checkout -b feature-zhanghao

4.本地分支与远端分支关联
> git push --set-upstream origin feature-zhanghao

5.修改本地文件，并提交
> git add .

6.增加commit,说明提交了什么
> git commit -m "提交个什么"

7.提交到远端仓库的的对应分支
> git push 

##### 日常提交
1.保证自己本地分支的代码都提交了，拉远端修改
> git pull

2.拉master上最新代码(因为我可能会直接改master)
> git merge origin/master

3.如果和有冲突需要合并冲突,修改文件，若本地有改动，直接执行上面第5步，无改动执行上面第7步
