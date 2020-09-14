## iToken的生成方式是怎样的？

将USDC/USDT/DAI/yCRV/ETH等资产存入YFII机枪池，就可以获得对应币种的iToken。如充值USDC则可以兑换出iUSDC。


## iToken代表什么含义？

iToken可以理解成YFII机枪池的权益Token，代表你在该机枪池的权益份额。以USDC为例，存入1000枚USDC可以得到略少于1000枚iUSDC，如果当前价格是1 iUSDC = 1.01 USDC，那么你可以铸造出1000/1.01 = 990 iUSDC。如果整个机枪池内共有99000枚iUSDC，那么代表你拥有该池全部USDC总额的1%。


## iToken的价值为什么会自动增长？

因为YFII机枪池挖矿都是本金无损策略，目标矿池的收益会自动换成本币Token回到池内，而此时iToken数量不变。这样池内的iToken可以兑换的Token就会变多，导致iToken价格上涨。


## 还有什么办法获得iToken?

普通用户参与DeFi理财，除了参与YFII机枪池，存入Token生成iToken这种方法以外，还可以直接通过Uniswap购买。根据YIP5，YFII利润的5%会进入循环矿池，这部分YFII应该会激励 iUSDT/USDT，iUSDC/USDC，iDAI/DAI 以及iETH/ETH，iBTC/wBTC等交易对。用户通过抵押这些交易对的UNI_LP进入循环矿池，来挖取额外YFII。届时会出现足够深度的交易对来支持用户通过购买iToken而实现理财。


## iToken的作用？

iToken最大的作用是阻止已进入YFII Vault的资金外流。当用户需要资金时候，iToken无须从机枪池提取本金（目前设置0.2%的提现费），而选择直接通过Uniswap交易成Token就可以了。iToken价值会恒定高于Token，只不过后面价格增长速度可能会慢下来。因为池内资金越多，APY也会被稀释的越厉害。0.2%提现费的设计，一方面是防止巨鲸稀释，另外一个作用就是锁定AUM（管理资金）。


## iToken/Token做市存在哪些优点？

1. 因为iToken/Token的汇率变化很慢，做市商的无偿损失会控制在很低范围内。如果支持Balancer挖矿，还可以获得BAL的双挖奖励。
2. 增加用户参与YFII理财的便利性，一键买入iToken即可完成，比存入Vault还更节省gas费。
3. 铸造iToken与购买iToken之间会出现价差，存在套利空间。当有人大量买入iToken的时候，价格上升，会有套利者代理铸造iToken，并注入交易对抹平套利空间。这个过程铸造了更多的iToken，有利于扩大YFII机枪池的AUM。


## iToken有可能衍生出哪些业务？

1. 因为iToken/Token汇率会始终高于1，可以考虑加入杠杆做借贷。在支持iToken的借贷平台内抵押iToken就可以1：1借贷出Token。具体操作来说：1000 USDC 抵押进入YFII Vault，可获得 990 iUSDC，再把990iUSDC拿到借贷平台进行抵押，可换出990 USDC；再次把990 USDC存入机枪池，换取980iUSDC，再进行抵押借贷... 依此循环，那么Token可以撬动多倍于本金的资产来进行理财，当然达成此条件需要借贷平台的USDC足够多，相当于用户从DeFi市场上搬运USDC到YFII平台，从而提高YFII的管理资金规模。
2. 借鉴yCRV系统的两部分收益：yToken的自动优化配置理财收益，以及curve的兑换手续费。那么iUSDC/iUSDT/iDAI三种资产可以合成为iCRV，既能获得iToken的自动挖矿策略收益，又可以获得后续Curve平台的稳定币互换手续费收益。iToken和iCRV未来也会有多种与其他DeFi项目的组合方式。


## iToken对YFII币价有哪些好处？

YFII 机枪池的特点是会循环递归的去挖矿的（复利），所有机枪池管理资金（AUM）产生利润的10%，都会用于回购YFII，发送至开发者基金，保险基金等。最初YFII机枪池的策略是100%回购，仅在资金量不大的时候有效；接下来的新版机枪池是通过增加资金管理规模（AUM）来提升YFII回购价值，即使10%也是很大的比例。iToken代表了管理资金规模，iToken发行量越大，机枪池获得利润就越多，带动10%的YFII回购从而提升币价。所以，YFII所有这些iToken都是为YFII币价提升服务的。
