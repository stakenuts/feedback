## Shelley Incentivised Testnet

This short document should document the feedback from the Shelley incentivised testnet.

### Last minute undelegation attack

A possible attack could consist of a bad player delegating to a legitimate pool α to trigger its oversaturation
limit and incentivising the delegators to move away from this pool over the duration of the epoch, but redelegating
its stake from the pool α just few instances before the epoch ends. The pool α would lose its weight in block creation.

A possible solution to this attack would be to put in place a rest period before each epoch of a specific duration and pick the distribution state randomly from this time interval. The delegators would be advised to make their distribution final before this rest period would take in place but would still have chance to react to a possible attack of this type. The bad player would also have less flexibility as the snapshot of the distribution would be presented as a time frame.

### Delegation causality problem

Stake delegation to different pools is one of the main element that keeps the network stable and secure. Once
a bad player is in the game and is identified by the stake holders, the incentive for them is to redelegate to
honest players in order to keep the network stable and secure and therefore protect their interests. However, as 
we have seen during the Shelley incentivised testnet, a number of bad players were able to destabilize the network
by producing a lot of lot of different same leade blocks for one slot and forcing the network into a lot of forks. 

After the issue has gain publicity, the delegators, including IOHK, were able to switch their stake to different staking
pools but we unable to do so due to the network instability. Therefere the bad player owned the stake and the delegators were
not possibile to execute their incentives.
