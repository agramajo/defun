# Defun

## Notes

1.
talk about percents, we can set diffent for buy/sell
it is more easy for contract if it only use integer numbers

for example MRI only has SELL taxes

buy
 prizepot 4
 lp 2
 dev 2

sell
 prizepot 4
 lp 2
 dev 2


only take fees on buys/sells not wallet transfers

totalSupply = 1 000 000 000

2.
need prizepot wallet
need dev wallet


## Internal notes

set uniswap v2 router

swapTokensAtAmount 

limitsInEffect -> true
  Check tradingActive
  Check transferDelayEnabled
  Check maxTransactionAmount (to)
  Check maxWallet (to)

  enableTrading()  -> tradingActive true, swapEnabled true
  removeLimits() -> limitsInEffect false
  disableTransferDelay() -> transferDelayEnabled false

  updateSwapEnabled() -> swapEnabled (VALUE)

