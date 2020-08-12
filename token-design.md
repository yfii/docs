## Token design of YFII 

![LOGO](./img/logo.png ':size=20%')

The total supply of YFII is **40,000**. Each of the two pools will be emitting 20,000 tokens to yield farmers, starting at 10,000 in the first week **halving every 7 days**. The number of tokens farmed is in proportion to the liquidity farmers provide to the pools. YFII will be completely distributed in the following 10 weeks.

![](./img/halvingModel.png ':size=90%')


## Burning of admin key

People may be worrying that if the developers would issue infinite number of YFII tokens to steal their money. The answer is: **impossible**. The minting keys have already been burnt by transferring the admin role to the blackhole address (0x00) so that no one has this privilege to mint new tokens. You can examine the burning txns below which are also documented at a specific [page](https://burn.yfii.finance/).

**YFII Token Governance Key**

https://etherscan.io/tx/0xd491dd5d190c6856f12cd88a8d318e71c5317371286379053a77040d09d27839

**Yearn Reward Distribution Key**

https://etherscan.io/tx/0xb78ff92dcdbc4fb2e69bfbd2aa2975d78e57983070c910121dbb77c03a28f53f

https://etherscan.io/tx/0x8d121a5dfd3808cb1ba8e5124dff01807c50a5fa769b77db7993eda6f4da38e8

**Balancer Reward Distribution Key**

https://etherscan.io/tx/0x26037582e80e9e668d8a8d16f7811441ff4db979ff63d0beb5c931c7fc9e7956

https://etherscan.io/tx/0x595088895e902fdbafb133c7d2b14e0264bfb4d400bb2928d27e1c10f4f05ac5

**addMinter record**

https://api.blockchair.com/ethereum/transactions?q=input_hex(%5E983b2d56),recipient(0xa1d0E215a23d7030842FC67cE582a6aFa3CCaB83)