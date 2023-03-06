1.  user:  await rewardRouter.connect(user0).mintAndStakeGlpETH(expandDecimals(299, 18), expandDecimals(299, 18), { value: expandDecimals(1, 18) })
2.  contracts/staking/RewardRouterV2.sol:mintAndStakeGlpETH()
3.  WETH(weth).deposit()
4.  IGlpManager(glpManager).addLiquidityForAccount()
5.  IRewardTracker(feeGlpTracker).stakeForAccount(account, account, glp, glpAmount)
6.  IRewardTracker(stakedGlpTracker).stakeForAccount(account, account, feeGlpTracker, glpAmount);
