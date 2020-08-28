### YFII机枪池支持币种：
**YFII vault机枪池挖矿**：YFII、DAI、yCRV、WETH、LINK-->xxx token-->YFII(代币抵押后自动挖矿并兑换成YFII分配用户)

**Pool1挖矿**：yCRV-->YFII（抵押稳定币yCRV挖YFII奖励）

**Pool2挖矿**：YFII/DAI -->BPT-->YFII（在Balancer通过YFII/DAI（2:98）交易对提供流动性获得BPT奖励，然后抵押BPT挖YFII）

### 1. YFII购买或兑换
YFII/DAI的交易对在Balancer深度最好，用DAI兑换时，建议使用Balancer。
ETH/YFII 的交易对在Uniswap深度最好，用ETH兑换YFII时，建议使用Uniswap。


#### 1.1 方法一：火币交易所购买YFII，然后提取到钱包（小白用户推荐）
#### 1.2 方法二：钱包里用Uniswap或Balancer兑换YFII
**图文教程：**

**以Uniswap为例**：[https://app.uniswap.org/#/swap](https://app.uniswap.org/#/swap?outputCurrency=0xa1d0E215a23d7030842FC67cE582a6aFa3CCaB83)

1）在钱包里找到Uniswap，连接上钱包

2）上面选 ETH，下方选YFII（或搜token地址：0xa1d0e215a23d7030842fc67ce582a6afa3ccab83）
![IMG_6817.jpg](./img/buy-token01.jpg ':size=40%')

3）填写数量，点击购买（swap）。在第一次使用时，可能会需要解锁（unlock）操作，会消耗少量手续费，解锁以后再点击购买（swap)。

4）设置手续费（最好比最高推荐gas高一点），然后提交确认。

![](./img/buy-token02.jpg ':size=40%')

#### Uniswap上兑换YFII视频教程：

[Uniswap上购买YFII教程.MP4](./video/buy-yfii.mp4 ':include :type=video')

### 2. DAI兑换

**方法一**：中心化交易所购买并提币到钱包

**方法二**：参考1.2方法，使用Uniswap或Balancer进行ETH与DAI兑换


另附：使用Uniswap兑换DAI视频教程：

[稳定币DAI对换教程.mp4 (5.3MB)](./video/buy-dai.mp4 ':include :type=video')


**方法三**：在 Maker 上 用ETH 抵押出 DAI


### 3. WETH兑换
#### 使用uniswap兑换WETH:
[https://app.uniswap.org/#/swap?outputCurrency=0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2](https://app.uniswap.org/#/swap?outputCurrency=0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2)


1）在钱包里找到uniswap，连接上钱包

2）上边选 ETH，下边选WETH

![](./img/buy-token03.png ':size=40%')

3）填写数量，点击购买（swap）。

4）设置手续费（最好比最高推荐gas高一点），然后提交确认。


### 4. LINK购买或兑换
#### 方法一：通过火币、Okex、币安、Coinbase等中心化交易所购买YFII，然后提取到钱包（小白用户推荐）


#### 方法二：使用Uniswap或Balancer兑换LINK

**图文教程：**

**以Uniswap为例**：

[https://app.uniswap.org/#/swap](https://app.uniswap.org/#/swap)

1）在钱包里找到Uniswap，连接上钱包

2）上面选 ETH，下方选LINK

![](./img/buy-token04.jpg ':size=40%')

3）填写数量，点击购买（swap）。在第一次使用时，可能会需要解锁（unlock）操作，会消耗少量手续费，解锁以后再点击购买（swap)。

4）设置手续费（最好比最高推荐gas高一点），然后提交确认。

![](./img/buy-token05.png ':size=40%')



### 5. yCRV兑换

**如果你的资金量在1万美元以上**：

首先进入Curve的Y池：[https://www.curve.fi/iearn/deposit](https://www.curve.fi/iearn/deposit) 抵押（**Deposit**）**USDT/DAI/USDC/TUSD** 任意一种币或多种币即可兑换出**yCRV**，也就是你的Y池权益Token。生成**yCRV**的交易费在0.15ETH左右，不建议小额资金使用。

参考以下Curve官网兑换yCRV视频教程：

[Curve官网兑换yCRV视频教程.MP4 (6.54MB)](./video/get-ycrv.mp4 ':include :type=video')

**如果你的资金量在1万美元以下：**

通过[**Uniswap**](https://uniswap.exchange/swap)兑换 **yCRV**更合适.

上方**ETH**, 下方输入**yCRV**

合约地址：**0xdf5e0e81dff6faf3a7e52ba697820c5e32d806a8**

![](./img/buy-token06.png ':size=40%')


### 6. sCRV兑换

生成流程与**yCRV**基本一致，只是少了**TUSD**，同时增加了一个**sUSD**入金方式，抵押（Deposit）后生成**sUSD Pool**权益Token，也就是**sCRV**

**生成地址：**[https://www.curve.fi/susdv2/deposit](https://www.curve.fi/susdv2/deposit)

![](./img/buy-token07.png ':size=40%')

**sCRV**目前在Uniswap上缺乏有深度的交易对，只能通过 curve.fi 发行获得。


### 7. cCRV兑换

生成流程与**yCRV**基本一致，仅支持**DAI**与**USDC**生成，入金后生成的是**Compound Pool**权益Token，也就是**cCRV**

**生成地址：**[https://www.curve.fi/compound/deposit](https://www.curve.fi/compound/deposit)

![](./img/buy-token08.png ':size=40%')

**cCRV**目前在Uniswap上缺乏有深度的交易对，只能通过 curve.fi 发行获得。

### 8. BPT（只适用Pool2挖矿）

BPT只能通过在Balancer提供流动性获得，具体可参考Pool2挖矿教程：[https://www.yuque.com/sawd49/faq/zkbgd0](https://www.yuque.com/sawd49/faq/zkbgd0)

#### 第一步：准备DAI

首先通过[Maker](https://oasis.app/borrow/)抵押资产生成**DAI**，或者交易所/Uniswap购买**DAI**
 
#### 第二步：抵押资产生成 BPT

[https://bal.yfii.finance/#/pool/0x16cAC1403377978644e78769Daa49d8f6B6CF565](https://bal.yfii.finance/#/pool/0x16cAC1403377978644e78769Daa49d8f6B6CF565)
点击以上链接进入页面后，提示先建立**Balancer Proxy**
a) 如果你有**YFII**，选择多资产抵押（**All Pool Assets**）
Unlock **DAI**以及 **YFII**（合约地址 **0xa1d0E215a23d7030842FC67cE582a6aFa3CCaB83** ）共发送两笔交易，使其变为已解锁状态。然后，在**Deposit Amount**中输入要抵押的**DAI**或**YFII**，输入其中一个数值，系统会自动帮你测算出要抵押的另一个数值。选择**Add Liquidity**发送交易即生成BPT

![](./img/buy-token09.png ':size=70%')

b) 如果你没有**YFII**，选择单资产抵押（Single Asset），解锁DAI并Deposit，选择Add Liquidity，系统会自动帮你兑换对应数量的**YFII**并抵押，同时生成BPT

![](./img/buy-token10.png ':size=70%')



