
# BTC whitepaper impression 

## 去中心化

基于POW的去中心化是BTC最重要的特性。BTC创造了资产（账本），同时以去中心化的方式保证了这种资产的安全性。
只要去中心化不被摧毁，用户便真正拥有资产的所有权。
进一步延伸，则是个人数据的自主权，隐私等，这些在其他链上体现较多。


## 数学相关

### 密码学算法
Hash算法
加解密/签名

### 二项随机漫步 Binomial Random Walk
诚实链和攻击者链之间的竞争过程可以用二项随机漫步来描述。可看作一个离散随机过程，每一步的状态（差距）由随机事件决定。

### 泊松分布 Poisson Distribution
为了计算攻击者能否赶上诚实链，可以使用泊松分布来描述攻击者链的生成进度。

在某些条件下，当进行足够多的独立随机试验时，二项分布可以近似为泊松分布。这种关系叫做**泊松极限**（Poisson Limit）。
在大多数情况下，攻击者链和诚实链的区块生成是独立的事件，而且生成区块的概率（每个矿工发现新区块的概率）相对较低，因此可以使用泊松分布来近似描述攻击者的进度
假设诚实链的区块生成符合期望时间，即按期望时间生成每个区块。而攻击者链的区块生成速率可以视为一个泊松过程，其中每个区块的生成时间间隔服从指数分布，因此，攻击者在一定时间内生成区块的数量服从泊松分布。