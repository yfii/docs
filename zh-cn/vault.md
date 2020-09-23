## vault 介绍


vault 合约信息都在 https://raw.githubusercontent.com/yfii/yvault/master/contracts/standard/v2/config.json

abi在：https://github.com/yfii/yvault/raw/master/abi/ivault.json

apy在: https://api.dfi.money/apy.json

第三方对接只需要与 vault合约对接就可以了

vault合约本身是兼容erc20的,名字都是iToken 如存入的是USDT则返回的是iUSDT

iToken的价格是不断增长的. 持有就会一值增值.


## vault合约交互

### 入金 (需要先对vault合约授权)

存入指定数量的代币到vault `function deposit(uint _amount)` 
（eth是例外的,可以直接转账给vault合约） 

存入以后会按照汇率返回指定的iToken数量.  

查看用户有多少iToken `function balanceOf(address user) public view returns (uint256)` 

iToken可以交易、转账，后续会开通iToken/Token lp的挖矿.

## 出金


1. 可以直接通过uniswap换回去(目前还没有激励流动性挖矿)
2. 通过合约兑换回去
    `function withdraw(uint amount)`  这边的amount是iToken的数量
    （取eth是例外的，方法名字是withdrawETH,withdraw是取weth出来）

## 如何计算Token 换到iToken的数量

1. 拿到 _pool = `function balance() public view returns (uint)`
2. 拿到 totalSupply = `function totalSupply() public view returns (uint)`
3. _amount为Token的数量. 换得iToken的数量为 _amount*totalSupply/_pool

## 如何计算iToken 可以换到多少Token

1. 拿到getPricePerFullShare =`function getPricePerFullShare() public view returns (uint)`
2. _amount为iToken的数量.换得Token的数量为 _amount*getPricePerFullShare/1e18


