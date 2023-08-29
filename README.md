### 个人介绍

##### 姓名：王众民       性别：男

##### 学历：大专       16年毕业

##### 邮箱：<wzmwzm1@126.com>

##### Github：<https://github.com/EndOfMaster>

##### Gitlab: <https://gitlab.com/EndOfMaster>

### 个人能力

- 接近三年智能合约开发经验，熟悉生态工具和语言如: solidity、hardhat 以及插件、ethers、truffle、node、web3js
- 5年java开发，标准java开发生态，如spring、sql、maven、gradle等
- 集群运维，如docker、k8s、gitlab runner等自动化运维
- 前端非样式开发，vue、element

### 期望职位

以太类区块链开发，远程或者北京

---

### 工作经历

##### dforce

##### 2021.10-2023.6.28       solidity智能合约开发

#### 项目介绍

dForce is a decentralized stablecoin protocol powered by an integrated DeFi matrix (assets, lending, trading and bridge).

dForce is backed by a number of world class investors (CMBI, Multicoin Capital, Huobi Capital), and are deployed on 8 networks currently, including Ethereum, Arbitrum, Optimism, BSC, Polygon, Avalanche, KAVA, and Conflux.

#### 参与项目
##### Ethereum mainnet veDF开发
分普通staking合约的sDF和无法交易只能投票的veDF，有manager分节点记录锁仓信息，有处理函数处理到期锁仓
##### aggregator合约以及后端服务开发
聚合1inch，dodo，curve，lsr，univ2，univ3的协议，以及后端服务接入为前端提供调用聚合合约的data
##### 聚合saddle和uniswap 优势的amm合约开发
结合saddle的sol重写curve的stable协议和uniswap的volatile协议，中间使用合约协调，而且都使用factory clone合约

#### 连接

[https://dforce.network](https://dforce.network/)

<br>

##### 北京纬颐科技有限公司

##### 2021.5-2021.10       solidity智能合约开发

#### 项目介绍

1类用户自定义创建资金池，自定金资金池预言机；2类用户进行杠杆买多买空，发放nft的购买凭证。后续功能以及设计:

1.  factory创建资金池，配置token、参数以及预言机，为nft合约沟通不同资金池提供router功能
2.  资金池内下单、平仓以及超越爆仓阈值的强平
3.  nft合约沟通业务功能，以及常规的展示功能

### 使用技术

solidity + node + truffle + openzeppelin

#### 工作内容

1.  完成合约的内部功能
2.  编写truffle部署脚本以及测试用例

<br>

##### 北京葫芦简医科技有限公司

##### 2020.3-2021.3       后端+运维

#### 项目介绍

平台旨在通过互联网手段建立高效的医患交流平台，通过知识社交，采用目前最流行的短视频、文章、直播等形式，推广健康知识科普，采用即时音视频通讯等方式搭建用户与医生之间的桥梁，最好诊前咨询，诊后服务，以达到在一定程度上缓解全社会医疗资源短缺、提高医疗工作者行医效率的目的。

1.  主服务分为client、member、media、community、diagnose五个服务
    - client为所有服务总出口，接口都在这里
    - member为账户系统服务，包括用户账户、钱包等功能
    - media为媒体服务，包括直播、小视频、文章等功能
    - community为社群相关服务，社群为医生创建的群，会在群内发布社群相关医疗信息，用户可以付费入群
    - diagnose为咨询服务，用户可以购买医生的电话咨询资格，或者在线交流的方式，购买社群也会获得医生设置的赠送次数
2.  管理后台分为新旧两个
    - 旧管理后台是项目之初使用springmvc+jsp的项目，包含了大部分管理功能以及查看功能
    - 新管理后台是vue编写的调用主服务接口中的纯web项目
3.  客户端分为医生端和用户端，有APP、小程序以及web页面

#### 使用技术

- springboot + mybites + dubbo + maven
- mysql + redis + es
- jenkins + docker

#### 工作内容:

1.  修复项目原有bug
2.  开发围绕直播相关的运营功能，如：观众数据分析、直播机器人（根据策略进出直播间、随机发聊天消息）、观看直播奖励等
3.  修改部分业务数据实体，包括重新设计、无缝替换和旧数据迁入
4.  将部分业务线运维修改为自动容器
5.  新功能的新旧管理后台配套管理功能

<br>

##### 北京中渡科技有限公司

##### 2018.5-2020.3       后端负责人

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

1.  从0到1的配合产品、UI、运营来设计项目新功能，服务模块，业务功能，分配组员工作内容
2.  设计整体服务架构和部分数据实体
3.  旧系统筛选、修改、重构、合并到新架构中

<br>

##### 北京积分客科技有限公司

##### 2017.8-2018.5       java开发

#### 项目介绍

线下商户收单系统，以及会员营销，包括：<br>

1.  用户的支付服务，以及支付后的运营页面
2.  商户的微信公众号以及pc的管理后台
3.  内部的管理后台

#### 使用技术

- springboot+ springdata + gradle
- mq + mysql + redis + mongo
- swarm + docker

#### 工作内容:

1.  根据需求不断接入新支付通道
2.  开发营销功能，比如：卡券、团购等
3.  商户管理后台以及管理后台的数据查询、分析等功能开发
4.  重构旧服务以解决服务器开销

<br>

##### 沛应云科技(北京)有限公司

##### 2016.8-2017.5       java开发

#### 项目介绍

线上及线下聚合支付系统<br>
总共接入了43种支付方式，用户在管理后台填入相应支付通道支付参数，可以只接入一次就可以得到多种支付方式，节省开发时间，也提供代申请支付通道等服务

#### 使用技术

- springboot+ springdata + gradle
- mq + mysql + mongo
- swarm + docker

#### 工作内容:

1.  接入新支付通道
2.  商户管理后台以及管理后台的数据查询、分析等功能开发

---

### 个人和社区以及创业项目

#### 加密艺术驱动器

#### 项目介绍

「加密艺术驱动器」是数字化合物推出的加密原生艺术作品，由10,000件NFT组成。

每件NFT的持有者有权在Nervos公链上通过行权，为词库增加一个词汇。NFT持有者将根据打开作品的时间不同而多次获得驱动器屏幕显示的随机词组，并有1次机会将喜欢的词组固定在屏幕上，这个动作也将被区块链确认，无法更改。

「加密艺术驱动器」把链上共建、参与者博弈作为艺术语言，赋予参与者权力，与创作者共同构建链上去中心化的「共同知识库」。

NFT持有者在元规则下拥有充分的主权和自由，用艺术的方式回应什么是「公链」、什么是「共同知识库」，以及如何在「共识」的机制下参与创造数字生活。

#### 参与部分

完整的合约开发和测试，功能包括：

- 收费铸造，但是随机给予不同稀有度级别的nft
- owner可以刷新驱动器词汇，并且可以锁定和向词汇池添加词汇
- 词库合约单一职责的管理词汇，包括添加，查询和随机抽取

#### 连接

<https://digitalcompound.org/#/projects/crypto-art-driver>
<https://opensea.io/collection/crypto-art-driver> <br>

#### wejuai

#### 项目介绍

带有隐私性的贴吧或者论坛项目
站酷上UI级项目介绍连接 <https://www.zcool.com.cn/work/ZNTM2MDgwNDg=.html>
源网址为 wejuai.com, 小程序为“为聚爱”，现在停止运营开源代码

#### 链接

<https://github.com/wejuai> <br>

#### amm mev

#### 项目介绍

- 自我研究的内容，主要是套利，是个人未来研究方向
- 目前有极少的成功次数

<br>

#### wkswap

#### 项目介绍

稳定币借贷，可以质押和借贷，存款和借款都会产生利息，利率根据总存款和总借款动态计算，可以质押一种代币同时借款多种代币，会计算仓位安全值，提供了清算接口，可以让清算人来清理即将爆仓的借款。<br>
清算奖励的1%会存入奖励池来做后续扩展

##### 链接

<https://github.com/wkswap/wkswap-protocol> <br>

#### AGIC

#### 项目介绍

区块链项目，质押eth铸币同时生息，抽取利息的5%存入资金池，发布股权卡nft，根据面额可以提取资金池中的利息

- 合约只发布到了kovan
- vue编写页面，有自适应和i18n功能，使用web3调用合约
- 后端服务使用node记录订单和监听合约事件

##### 使用技术

- solidity + node + vue + web3
- mongo

##### 连接

[Agic.link](https://agic.link/)

<br>

#### 峰链凭证

#### 项目介绍

一种部署在招行一链通的购买、交易、核销的nft凭证<br>
由于可能无法使用ipfs等文件存储技术，采用了和uniV3一样的链上返回生成的svg图片模式

##### 使用技术

- solidity + node + web3
- 独立运行仿evm节点

##### 连接

<https://github.com/nipeak/nipeak-digital-copyright-cmbchain>

<br>

#### Let's ssl

#### 项目介绍

使用Let's Encrypt签名证书，分为后端和前端两部分

- vue编写页面，有自适应
- 后端服务使java调用相关接口

##### 使用技术

- java + vue
- mysql

##### 连接

[LetsSSL.com](https://letsssl.com/)

---

