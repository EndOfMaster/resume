### 个人介绍
##### 性别：男
##### 学历：大专 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 16年毕业
##### 邮箱：wzmwzm1@126.com
##### Github：[https://github.com/EndOfMaster](https://github.com/EndOfMaster)
##### Gitlab: [https://gitlab.com/EndOfMaster](https://gitlab.com/EndOfMaster)

### 个人能力

- 5年java开发，标准java开发生态，如spring、sql、maven、gradle等
- 集群运维，如docker、k8s、gitlab runner等自动化运维
- 自学以太类开发生态，如sol、node、web3、vue

### 期望职位
以太类区块链开发，远程或者北京

### 个人项目
##### AGIC
##### 2020.9-2 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 全栈

#### 项目介绍
区块链项目，质押eth铸币同时生息，抽取利息的5%存入资金池，发布股权卡nft，根据面额可以提取资金池中的利息

- 合约只发布到了kovan
- vue编写页面，有自适应和i18n功能，使用web3调用合约
- 后端服务使用node记录订单和监听合约事件

#### 使用技术
- sol + node + vue + web3
- mongo

#### 连接
[Agic.link](https://agic.link/)

<br>

##### Let's ssl
##### 2020.2-2020.3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 全栈

#### 项目介绍
使用Let's Encrypt签名证书，分为后端和前端两部分

- vue编写页面，有自适应
- 后端服务使java调用相关接口

#### 使用技术
- java + vue
- mysql

#### 连接
[Let's SSL.com](https://letsssl.com/)

### 工作经历

##### 北京葫芦简医科技有限公司
##### 2020.3-2021.3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 后端+运维
#### 项目介绍
平台旨在通过互联网手段建立高效的医患交流平台，通过知识社交，采用目前最流行的短视频、文章、直播等形式，推广健康知识科普，采用即时音视频通讯等方式搭建用户与医生之间的桥梁，最好诊前咨询，诊后服务，以达到在一定程度上缓解全社会医疗资源短缺、提高医疗工作者行医效率的目的。

1. 主服务分为client、member、media、community、diagnose五个服务
    - client为所有服务总出口，接口都在这里
    - member为账户系统服务，包括用户账户、钱包等功能
    - media为媒体服务，包括直播、小视频、文章等功能
    - community为社群相关服务，社群为医生创建的群，会在群内发布社群相关医疗信息，用户可以付费入群
    - diagnose为咨询服务，用户可以购买医生的电话咨询资格，或者在线交流的方式，购买社群也会获得医生设置的赠送次数
2. 管理后台分为新旧两个
    - 旧管理后台是项目之初使用springmvc+jsp的项目，包含了大部分管理功能以及查看功能
    - 新管理后台是vue编写的调用主服务接口中的纯web项目
3. 客户端分为医生端和用户端，有APP、小程序以及web页面

#### 使用技术

- springboot + mybites + dubbo + maven
- mysql + redis + es
- jenkins + docker

#### 工作内容:
1. 修复项目原有bug
2. 开发围绕直播相关的运营功能，如：观众数据分析、直播机器人（根据策略进出直播间、随机发聊天消息）、观看直播奖励等
3. 修改部分业务数据实体，包括重新设计、无缝替换和旧数据迁入
4. 将部分业务线运维修改为自动容器
5. 新功能的新旧管理后台配套管理功能

<br>

##### 北京中渡科技有限公司
##### 2018.5-2020.3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 后端负责人

#### 项目介绍
- 分为 4 端为旅行社、导游、用户、控制台，旅行社可以给导游下单带团，用户 也可以预约导游空闲时间来
进行自由行，用户也可以发布自驾游需求，来自行找同伴同游。有 多业务核心，支付核心，异步处理模块，第
三方服务模块。
支付核心分为 gateway 和 sync，gateway 接入多个支付通道，包括微信、支付宝以及 PayPal， 多个需求
支付的项目使用 spring rest template 内网远程请求 gateway，保证了安全性，sync 接收支付 通道的异步通
知以及使用 mq 主动查询双方式来确认订单完成状态，并且解决重入问题，最后 再通知原项目请求方支付完
成。
- 异步处理模块把无需下单时立即处理的业务内容异步处理，同时处理一些定时处理的业务。 ·多业务核心
为四个用户端独立业务模块独立服务，提高可扩展性，和方式关键功能被高并发 的用户请求堵塞。
- 第三方服务模块是请求第三方服务接口的独立服务，用来刷新 token，存储各种第三方请求 密钥及加密签
名方式，这样业务服务无需考虑复杂第三方请求参数以及加密签名，只需要考虑 业务功能即可。

#### 使用技术

- springboot+ springdata + gradle
- mq + mysql + redis + mongo
- k8s + docker

#### 工作内容:
1. 从0到1的配合产品、UI、运营来设计项目新功能，服务模块，业务功能，分配组员工作内容
2. 设计整体服务架构和部分数据实体
3. 旧系统筛选、修改、重构、合并到新架构中

<br>

##### 北京积分客科技有限公司
##### 2017.8-2018.5 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; java开发

#### 项目介绍
线下商户收单系统，以及会员营销，包括：<br>
1. 用户的支付服务，以及支付后的运营页面
2. 商户的微信公众号以及pc的管理后台
3. 内部的管理后台

#### 使用技术

- springboot+ springdata + gradle
- mq + mysql + redis + mongo
- swarm + docker

#### 工作内容:
1. 根据需求不断接入新支付通道
2. 开发营销功能，比如：卡券、团购等
3. 商户管理后台以及管理后台的数据查询、分析等功能开发
4. 重构旧服务以解决服务器开销

<br>

##### 沛应云科技(北京)有限公司
##### 2016.8-2017.5 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; java开发

#### 项目介绍
线上及线下聚合支付系统<br>
总共接入了43种支付方式，用户在管理后台填入相应支付通道支付参数，可以只接入一次就可以得到多种支付方式，节省开发时间，也提供代申请支付通道等服务

#### 使用技术

- springboot+ springdata + gradle
- mq + mysql + mongo
- swarm + docker

#### 工作内容:
1. 接入新支付通道
2. 商户管理后台以及管理后台的数据查询、分析等功能开发
