# LINUX Refund Methodology

This document outlines our proposed methodology for refunding users who participated in the $LINUX token auction and launch. Supporting data and WIP calculations are also soon be made available in this repo.

Please note that this is a living document. Our approach and results may change over time as we work with the community to refine the methodology.

## Context

On 28 May 2025, we announced that we would be retiring the $LINUX token and refunding users who participated in the $LINUX token launch. See our post <TOADD> for details.

## Recovered assets

As of the writing of this document, we (the GitFish team) are in possession of:

- <TOADD> SOL withdrawn from the liquidity pool
- 438.24 SOL in auction fees, transferred to the admin wallet after token launch

25% of the auction fees, or 109.56 SOL, has been pledged as a referral bonus to users who referred their friends. In other words, a total of <TOADD> + 109.56 = <TOADD> SOL is recovered and can be returned to users. 

All present and future LINUX tokens in our wallet will not be redistributed and should be considered retired. 

## Refund methodology

The core principle of our approach is to try to put users back in the position they would have been in had the launch not gone ahead. In other words, the amount of compensation for each user is based on:

1. the amount in SOL they paid to buy the token, less
2. the amount in SOL they received from selling the token

We propose to compensate users based on a payout in two steps:

1. First, we will refund all users who bought LINUX tokens either in the auction or after launch, and never sold
2. Second, we will distribute the remaining LINUX tokens to users who sold some or all of their tokens

Let's step through each scenario for what users could have done with their tokens after launch, and explain how we calculate the refund for each case.

### Scenario 1: Bidder did not collect their tokens

A bidder who did not collect their tokens after launch will be eligible for a full refund of the amount they paid for the tokens. 

Example A:
- User paid 1 SOL for 1000 LINUX tokens
- User did not collect their tokens
- User is eligible for a refund of 1 SOL

### Scenario 2: Bidder collected their tokens and held onto them

A bidder who collected their tokens and held onto them will be eligible for a full refund of the amount they paid, provided they transfer the tokens back to the GitFish admin wallet `EX7QGHSreah6EUtsPXCcen5R8JUyiVQWgz6aV4UspyMy`.

Example B:
- User bought 1000 LINUX tokens with 1 SOL
- User collected their tokens and held onto them
- User transfers the tokens back to the GitFish admin wallet
- User is eligible for a refund of 1 SOL

Example C:
- User bought 1000 LINUX tokens with 1 SOL
- User collected their tokens and held onto them
- User does not transfer the tokens back to the GitFish admin wallet
- User is not eligible for a refund

### Scenario 3: User did not participate in the auction but bought tokens after launch and held onto them

A user who did not participate in the auction but bought tokens after launch and held onto them will be eligible for a full refund of the amount they paid for the tokens. They are treated similarly to a bidder who collected and held onto their tokens after launch (see Scenario 2).

The amount of compensation leftover after paying out users in Scenarios 1-3 will be distributed to remaining users in proportion to their realized losses.

### Scenario 4: User sold some or all of their tokens

A bidder or buyer who sold some or all of their tokens will be eligible for a partial refund, based on the amount of their loss. Note that as with users in Scenario 2, they will need to transfer remaining token balances back to the GitFish admin, or they will forfeit their right to a refund on those balances.

Example D:
- User bought 1000 LINUX tokens with 1 SOL
- User sold 500 LINUX tokens for 0.3 SOL
- User sold 500 LINUX tokens for 0.2 SOL
- User is eligible for a maximum refund of 1 - 0.3 - 0.2 = 0.5 SOL (less if claims exceed recovered assets)

Example E:
- User bought 1000 LINUX tokens with 1 SOL
- User sold 500 LINUX tokens for 0.3 SOL
- User transfers remaining 500 LINUX tokens back to the GitFish admin wallet
- User is eligible for a maximum refund of 1 - 0.3 = 0.7 SOL (less if claims exceed recovered assets)

Example F:
- User bought 1 SOL for 1000 LINUX tokens
- User sold 500 LINUX tokens for 0.3 SOL
- User does not transfer remaining 500 LINUX tokens back to the GitFish admin wallet
- User is not eligible for a refund

### Scenario 5: User traded their tokens

A user who traded (i.e. bought and sold) LINUX tokens will be eligible for a partial refund. Where a user placed multiple buys and sells, we apply the First-In-First-Out (FIFO) approach to determine the user's cost basis and realized losses. As with users in Scenario 4, they will need to transfer remaining token balances back to the GitFish admin to be eligible for a refund on remaining LINUX balances.

Example G:
- User bought 1000 LINUX tokens with 1 SOL
- User sold 200 LINUX tokens for 0.15 SOL
- User bought 400 LINUX tokens for 0.2 SOL
- User sold 1200 LINUX tokens for 0.15 SOL
- User is eligible for a maximum refund of 1 - 0.15 - 0.2 - 0.15 = 0.5 SOL (less if claims exceed recovered assets)

Example H:
- User bought 1000 LINUX tokens with 1 SOL
- User sold 200 LINUX tokens for 0.15 SOL
- User bought 400 LINUX tokens with 0.2 SOL
- User transfers remaining 1200 LINUX tokens back to the GitFish admin wallet
- The realized loss on the 200 LINUX tokens is 0.15 - 0.2 = -0.05 SOL
- The cost basis for the 1200 LINUX tokens is:
  - 800 LINUX tokens for 0.8 SOL
  - 400 LINUX tokens for 0.2 SOL
- User is eligible for a maximum refund of 0.05 + 0.8 + 0.2 = 1.05 SOL (less if claims exceed recovered assets)

### Scenario 6: User added their tokens to a liquidity pool

A user who added their tokens to a liquidity pool will be treated similar to a trader in Scenario 5. Each pair of deposit and withdrawal actions is treated as a trade. If the user does not withdraw LP and transfer remaining tokens back to the GitFish admin, they will not be eligible for a refund.

### Scenario 7: User transferred their tokens to another wallet

A user who transferred their tokens to another wallet will have their refund transferred to the new wallet, not the old one.

Example I:
- User A paid 1 SOL for 1000 LINUX tokens
- User A transferred 1000 LINUX tokens to User B
- User B transfers 1000 LINUX tokens back to the GitFish admin wallet
- User B is eligible for a refund of 1 SOL