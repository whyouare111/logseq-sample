---
title: The MVP Before Christmas
---

## 来源 https://dev.mirror.xyz/J1RD6UQQbdmpCoXvWnuGIfe7WmrbVRdff5EqegO1RjI
### 对应的 Arweave 存储 https://4y3qyvn34whoszbepxgnssldfclem5uthkb34jj4amysp67pl6ta.arweave.net/5jcMVbvljulkJH3M2UljKJZGdpM6g74lPAMxJ_vvX6Y
## 如何构建一个 Web3 原生的写作平台
### 首先面临的一个挑战是，从 web3 的角度思考如何搭建平台。以下是 web3 的游戏规则（ via negativa 式，即 “它不是什么/它不应该如何”）
#### 1. 帖子内容不应该是中心化的
##### 使用 Arweave 来存储用户内容
###### 数据永久存储，只需在上传时支付一次性费用
###### 上传到 Arweave 的数据包括检索出版物的所有条目 （包括任何修改）和验证作者身份真实性所需的所有信息。
##### 计划发布协议规范和开源工具
###### 提升检索和验证的使用体验
##### 能够轻易地从 ^^Mirror^^ 中迁移出去
#### 2. 阅读体验不需要信赖  ^^Mirror^^
##### 所有条目用用户的签名密钥
###### 不是以太坊的密钥对，不包含任何直接的经济价值
####### 也就是说这个密钥是公开的形式也不会直接危害到钱包里的各种数字资产
##### 签名、签名过的摘要、签名的内容上传 Arweave
###### `authorship.signature`
###### `content.digest`
###### `content.body`
##### 签名密钥本身会被放入一个申明作者权利的消息中，然后由作者的以太坊地址进行签名。
###### 这些信息也会上传至 Arweave
####### 对应每个条目和更新。
###### `authorship.signingKeyMessage`
#### 3. ^^Mirror^^不应拥有作家的域名
##### [[ENS]]
###### 作家通过销毁一个 [[$WRITE]] Token 来声明对域名的所有权
####### [[$WRITE]] 用投票的方式来邀请 [[Twitter]] 用户
#### 4. 作家不需要连接他们的钱包并签署他们所写的一切
##### 我们不用很麻烦很累就能 <del>成佛</del> 写文章
#### 5. ^^Mirror^^不应尝试在浏览器端存储以太坊私钥
#### 6. 写作不应该太贵 （对 ^^Mirror^^ 或作家来说都是）
#### 7. 奖励： 不用邮箱-密码注册
### 架构图大致是这样
#### [架构图](https://images.mirror-media.xyz/publication-images/4ad92c52-5226-40c1-b654-4bbfe905c278.jpeg){:height 472, :width 604}
###
