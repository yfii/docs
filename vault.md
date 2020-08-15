## What is YFII Vault?

YFII Vault is a yield aggregator for farming pools that targets highest APR using a set of strategy contracts. Basically you deposit the token it supports and automatically get the yield that the strategy has farmed. Everyone is welcomed to write their own strategies and those with the highest votes from the community will be implemented. The Vault also saves you tons of gas during complex contract interactions because all you need to do is just deposit and withdraw.

## YAM strategy: A brief how-to

The first strategy online now is the one that farms YAM pools. Users deposit any one of SNX/LEND/MKR/AMPL/YFI/COMP/LINK/WETH tokens into the YFII vault and enjoy yileds of YFII tokens.

1. This guide supposes you choose to deposit WETH into the vault. First you have to swap ETH (or any other tokens you have) for WETH. Go to [UNISWAP](https://app.uniswap.org/#/swap), choose ETH in the *From* section and choose WETH in th *To* section. Input the number you'd like to swap and click wrap. The price is always 1:1.

![](./img/vault1.png ':size=40%')

2. Go to [YFII Vault page](https://vault.yfii.finance/) and expand the WETH section. You can see your balance of WETH on the left. Input the amount you'd like to deposit and then click *Deposit*. If it's the first time you deposit WETH you'll have to send an *approve* txn (see the popup window of Metamask). When it's approved, Metamask will popup again for you to send the actual *Deposit* transaction. After the txn has been confirmed you'll see your WETH balance on the right side which means you have such an amount of WETH in the vault which is farming the best yield according to our strategy.

![](./img/vault2.png ':size=70%')

3. You can claim your yield at any time by clicking the *Claim* button on the right. If you'd like to exit the Vault, click *Withdraw*. The transaction will also claim the yiled for you when exiting.