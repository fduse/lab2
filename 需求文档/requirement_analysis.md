# 图书馆管理系统 需求分析文档

## 系统开发总体目标

### 开发对象
图书馆管理系统

### 主要用户
读者（10万），前台人员，维护和财务等图书馆工作人员

### 系统组成
1. 交互系统
2. 借阅系统
3. 通知系统
4. 维护系统
5. 财务系统

### 预期效果

读者可凭借合法的居民身份证，在前台或自助终端办理借书证，并得到系统的登录凭证；或进行挂失补办等卡务操作。

读者可凭借登录凭证在 Web 端，或凭借登录凭证/借书证在前台或自助终端查询书籍信息，并对想借阅的书进行预约。

读者/前台可凭借借书证方便快捷地进行借还书、续借等操作。

系统可以检查读者的预约时间、还书期限等是否到达，并根据读者预留的个人信息向其发送提醒，以避免发生错过预约、违约等情况。

维护人员可利用隔绝了无关人员的专属安全系统进行新书录入，查询读者信息、书籍信息、借阅记录，修改系统参数等操作。

财务人员可利用系统管理书籍的可用性信息，并方便地决策报废。可利用系统自动计算的违约、损坏赔偿金额向读者收取违约金和赔偿。

### 项目预算
100万元人民币

### 部署环境
（暂不考虑）

## 数据模型
![类图](http://i.v2ex.co/A46ym9o0.png)

## 用况模型
### UML 用况图
![](http://ww3.sinaimg.cn/mw690/65381e00gw1f3lxvtzpqej20i10h5acn.jpg)

### UML 活动图
- 办证

![](http://ww3.sinaimg.cn/mw690/65381e00gw1f3mum4696bj209f0ej3yz.jpg)

- 挂失

![](http://ww2.sinaimg.cn/mw690/65381e00gw1f3mum6kxf0j20a30df0t3.jpg)

- 退卡

![](http://ww2.sinaimg.cn/mw690/65381e00gw1f3mumaa1bsj20cr0cbq3b.jpg)

- 登录

![](http://ww4.sinaimg.cn/mw690/65381e00gw1f3mum644wlj20ck09g74l.jpg)

- 修改个人信息

![](http://ww1.sinaimg.cn/mw690/65381e00gw1f3mumctfb5j20bu0grmxs.jpg)

- 查询书籍

![](http://ww1.sinaimg.cn/mw690/65381e00gw1f3mum4i551j206q08zdfx.jpg)

- 提醒

![](http://ww1.sinaimg.cn/mw690/65381e00gw1f3mum5663pj20h30bnaan.jpg)

- 借书

![](http://ww3.sinaimg.cn/mw690/65381e00gw1f3mum8ro23j20ex0irjs9.jpg)

- 还书

![](http://ww4.sinaimg.cn/mw690/65381e00gw1f3mum7e3yrj20ex0gjaaq.jpg)

- 预约

![](http://ww1.sinaimg.cn/mw690/65381e00gw1f3mumdxgvzj20ca0ix0tf.jpg)

- 续借

![](http://ww1.sinaimg.cn/mw690/65381e00gw1f3mumdih3lj20ex0f7wf3.jpg)

- 违约金缴纳

![](http://ww1.sinaimg.cn/mw690/65381e00gw1f3mumat0i8j208z0er3yw.jpg)

- 丢失损坏赔偿

![](http://ww1.sinaimg.cn/mw690/65381e00gw1f3mum9t06nj209n0ir74z.jpg)

- 后台数据查询

![](http://ww4.sinaimg.cn/mw690/65381e00gw1f3mum7zp94j209s0dfq39.jpg)

- 报废

![](http://ww2.sinaimg.cn/mw690/65381e00gw1f3mum9b3j1j208r0b7jrk.jpg)

- 系统参数修改

![](http://ww3.sinaimg.cn/mw690/65381e00gw1f3mumbkkv9j20dl0cjmxl.jpg)

- 新书录入

![](http://ww1.sinaimg.cn/mw690/65381e00gw1f3mumc6u5rj206q0bnq34.jpg)

## 数据流模型
- 0 层

![0层](http://i.v2ex.co/gS58tJ3C.png)

- 1 层

![0层](http://i.v2ex.co/4puQud1q.png)

## 行为模型
- 图书管理系统状态图

![图书系统状态图](https://github.com/fduse/lab2/blob/master/stateChart/system.png)

- 图书状态图

![图书状态图](https://github.com/fduse/lab2/blob/master/stateChart/book.png)

- 读者状态图

![读者状态图](https://github.com/fduse/lab2/blob/master/stateChart/reader.png)