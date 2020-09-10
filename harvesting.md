## What is harvesting?

When a vault is farming, it periodically sells its target tokens and buy back the principal tokens and YFII before distributing the yields to vault users. For example, a TUSD vault farming CRV will periodically sell CRV and buy TUSD with 90% of the CRV yields and buy YFII with the left 10% and then distribute these tokens according to the rules stipulated by [YIP-5](https://yips.yfii.finance/YIPS/yip-5). This process is called *harvesting* and an active vault needs to harvest from time to time.

Anyone can invoke the *Harvest* function to collect yields into the vault and in return get 1% of the yield from that batch. It may cost gas of approximately 0.1 ETH. Frequent harvesting can help reduce the slippage during token swaps and thus increase the whole income of the Vault. Please keep an eye on the current yield and also check if others have already invoked the function recently, or the rewards won't cover your gas fee.


## How to help harvest?

You are supposed to be familiar with how smart contracts work. Currently there is no front-end for the *harvest* function so you have to interact with the contracts using Etherscan or other CLI tools you like.

For example, if you want to harvest for the USDT vault, go to the [Write Contract page on Etherscan](https://etherscan.io/address/0xe2df4c46acabb1cdb446351d6b24727944a5bfcc#writeContract) of the strategy address. Then click Connect to Web3 to connect with your wallet.

![](./img/harvest1.png ':size=50%')

Find the 3rd function **harvest** and click **Write**. Accept the transaction in Metamask and when it's confirmed you have successfully helped harvest.

![](./img/harvest2.png ':size=20%')


## Strategy contracts

Here's a list of strategy contract addresses for each vault:

**USDT**: 0xe2df4c46acabb1cdb446351d6b24727944a5bfcc

**yCRV**: 0x898828957133d4c50030a5A2D55Ca370915E6A77

**DAI**: 0xbDD4a57c5EE8558370bb661d29a979657D81258e

**TUSD**: 0x30aE128ebCdec11F62cB3fa9C6a0E8269a9AF686