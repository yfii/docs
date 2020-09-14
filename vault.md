## What is YFII Vault?

YFII Vault is a yield aggregator for farming pools that targets highest APR using a set of strategy contracts. Basically you deposit the token it supports and automatically get the yield that the strategy has farmed. Everyone is welcome to write their own strategies and those with the highest votes from the community will be implemented. The Vault also saves you tons of gas during complex contract interactions because all you need to do is just deposit and withdraw.


## What is iToken?

iToken refers to a set of tokens that serve as proof of deposit in the vaults. Since version 2.0, users who deposit funds into the vaults will automatically get corresponding iTokens. For example, if you deposit USDT into the vault, it gives back iUSDT which is interest bearing. As the vault is generating yields, when you later return your iUSDT to withdraw your funds, you should get more USDT than you have deposited.

The fun part of iToken is that you do not have to withdraw your funds from the vault by yourself. The interest-bearing iTokens can be transferred or traded in the market. The price of an iToken in the original token (e.g., iDAI/DAI) is always above 1 and this number should be increasing all the time as long as the vault is generating yields. iTokens can also be used as collaterals for debts or staked for yield farming. That's the first step towards the world of DeFi LEGOs. You can read more about iToken [here](itokens.md).


## How to use the Vault?

### :fire: Version 2.0

1. Visit [DFI website](https://dfi.money/) and connect your wallet.

2. Choose the token you'd like to deposit and click the arrow to expand the corresponding section. This guide supposes you choose to deposit **DAI** into the Vault. On the left you'll see your balance in your wallet. Input the number you'd like to deposit. If it's the first time you deposit, click *Approve* to allow the contract to spend your **DAI**. After the *Approve* transaction is confirmed, the button will become *Deposit*. Click the *Deposit* button to deposit **DAI** into the Vault. After the txn is confirmed, your farming automatically starts and the Vault begins to generate yield for you.

![](./img/vault1.png ':size=70%')

3. You'll notice that after depositing **DAI**, you receive a token named **iDAI** in your wallet. It is the proof of your deposit; do not send it to others unless you mean to do so. As long as you are holding this **iDAI**, you are able to withdraw your deposit along with the interest at any time. If you send or sell **iDAI** to others, you are giving away your rights to withdraw the corresponding funds.


### Version 1.0
?> :bulb: [Old vaults of V1.0](https://v1.dfi.money/) are **DEPRECATED** as they do not generate yield anymore except for yCrv and cCrv. You are encouraged to take your funds out of the old vaults and deposit them into the new ones. 

> **Features**
>
> - In the past versions, a whale could make a sudden deposit to dilute others' incoming and then immediately withdraw its funds. Now this exploitation is no longer possible because the income will be emitted gradually in the following 24 hours after each deposit. For example, if a user claims the yield 8 hours after the last deposit transaction, he/she only gets 1/3 of the yield. Please note that the 24-hour countdown will be reset each time when the user deposits into the Vault.
>
> - Anyone can invoke the *Harvest* function to collect yields into the vault and in return get 1% of the YFII tokens in that batch. It may cost gas of approximately 0.1 ETH. Frequent harvesting can help reduce the slippage during token swaps and thus increase the whole income of the Vault. Please keep an eye on the current yield and also check if others have already invoked the function recently, or the rewards won't cover your gas fee.
>
> - When a new strategy is online, you do not need to transfer your funds to a new vault. The vault can automatically switch to the new strategy.

1. This guide supposes you choose to deposit WETH into the Vault. First go to the [new Vault website](https://dfi.money/) and connect your wallet. Click *Vault* to enter the Vault interface.

2. Expand **WETH** section and input the number you'd like to deposit. If it's the first time you deposit, click *Approve* to allow the contract to spend your WETH. After the *Approve* transaction is confirmed, the button will become *Deposit*. Click the *Deposit* button to deposit **WETH** into the Vault. After the txn is confirmed, your farming automatically starts and the Vault begins to generate yield for you.

![](./img/vault-new1.png ':size=70%')

3. You can see how many WETH you've deposited into the Vault in the *Deposited* section. You can withdraw at any time and when withdrawing, your yield (if there are any available) will be claimed at the same time. The *Earned* section displays how much you have actually earned in this Vault. You can claim your yield at any time without withdrawing your deposit. Please **note** that your claimable yield is released evenly in 24 hours after your last deposit. If you claim your yield within 24 hours, you only get a portion of it and the unclaimable part will be donated to YFII's development fund. The *Pending* section indicates the estimated yield to be harvested into the Vault (and to become your *Earned* balance).

![](./img/vault-new2.png ':size=70%')

4. An ordinary user can safely ignore the *Farm* and *Harvest* buttons. However, if you'd like to contribute to the community, you can spend your own gas to help the Vault send idle balance to the farm by clicking *Farm* button. You can also click *Harvest* to help the Vault finalize its pending earnings, and in return you'll be rewarded with 1% of the yield of that harvest.

![](./img/vault-new3.png ':size=70%')


### Legacy version

!> :bulb: **NB:** The [old vaults](https://vault.yfii.finance/) are not generating yields and will no longer be maintained. Please withdraw all your funds.