## What is YFII Vault?

YFII Vault is a yield aggregator for farming pools that targets highest APR using a set of strategy contracts. Basically you deposit the token it supports and automatically get the yield that the strategy has farmed. Everyone is welcomed to write their own strategies and those with the highest votes from the community will be implemented. The Vault also saves you tons of gas during complex contract interactions because all you need to do is just deposit and withdraw.

## How to use the Vault?

### YAM strategy

The first strategy online is the one that farms YAM pools. Users deposit any one of SNX/LEND/MKR/AMPL/YFI/COMP/LINK/WETH tokens into the YFII vault and enjoy yileds of YFII tokens.

1. This guide supposes you choose to deposit WETH into the vault. First you have to swap ETH (or any other tokens you have) for WETH. Go to [UNISWAP](https://app.uniswap.org/#/swap), choose ETH in the *From* section and choose WETH in th *To* section. Input the number you'd like to swap and click wrap. The price is always 1:1.

![](./img/vault1.png ':size=40%')

2. Go to [YFII Vault page](https://vault.yfii.finance/) and expand the WETH section. You can see your balance of WETH on the left. Input the amount you'd like to deposit and then click *Deposit*. If it's the first time you deposit WETH you'll have to send an *approve* txn (see the popup window of Metamask). When it's approved, Metamask will popup again for you to send the actual *Deposit* transaction. After the txn has been confirmed you'll see your WETH balance on the right side which means you have such an amount of WETH in the vault which is farming the best yield according to our strategy.

![](./img/vault2.png ':size=70%')

3. You can claim your yield at any time by clicking the *Claim* button on the right. If you'd like to exit the Vault, click *Withdraw*. The transaction will also claim the yiled for you when exiting.

### CRV strategy

The CRV strategy farms CRV tokens of Curve DAO by depositing yCRV (Y pool LP token of Curve) and automatically swaps CRV for YFII tokens as the final yield.

> ?> **New Features** :bulb:
>
> - In the past versions, a whale could make a sudden deposit to dilute others' incoming and then immediately withdraw its funds. Now this exploitation is no longer possible because the income will be emitted gradually in the following 24 hours after each deposit. For example, if a user claims the yield 8 hours after the last deposit transaction, he/she only gets 1/3 of the yield. Please note that the 24-hour countdown will be reset each time when the user deposits into the Vault.
>
> - Anyone can invoke the *Harvest* function to collect yields into the vault and in return get 1% of the YFII tokens in that batch. It may cost gas of approximately 0.1 ETH. Frequent harvesting can help reduce the slippage during token swaps and thus increase the whole income of the Vault. Use [this link](https://etherscan.io/address/0xfd4c75184bed2013fdb621f54885b2d2ed7c3894#writeContract) to harvest (UI to follow). Please keep an eye on the current yield and also check if others have already invoked the function recently, or the rewards won't cover your gas fee.

1. To farm with this strategy, you need to have yCRV in your wallet first. Go to [Curve's Y pool](https://www.curve.fi/iearn/deposit) and deposit any one or any combo of USDT/DAI/USDC/TUSD to get yCRV.

![](./img/vault3.png ':size=70%')

The above transaction may cost about 0.3 ETH worth of gas, so if you're playing with a small amount of fund you may want to buy yCRV directly on [Uniswap](https://app.uniswap.org/#/swap). Set the target token to 0xdf5e0e81dff6faf3a7e52ba697820c5e32d806a8 (yCRV) and swap.

![](./img/vault4.png ':size=40%')

2. Now you've got yCRV tokens. To join the Vault, go to [YFII Vault page](https://vault.yfii.finance/). Input the number of yCRV you'd like to deposit on the left side and then click *Deposit*. After the txn has been confirmed, the Vault starts to farm for you.

![](./img/vault5.png ':size=70%')
