# NLP (Nep5 Lottery platform)

NLP is the first purely decentralized smart contract lottery that lets users operate and maintain the lottery over their earnings. it aims to rectify the shortcomings in the traditional lottery in which the participation is limited and most funds are used in maintaining administrative costs.

## Contract type
Application

## Contract hash

ada839286d23cdfb42eb556461b9382d02b6e12f

## Methods

#### Core methods:
`buyLotteryTicket(args[])`

| Arg | type | Description
|--- |--- |--- |
| playerHash | string | Player script hash. |
| walletType | 1, 2 | If set 1, the contract transfers funds from the player. If set 2, from users balance in the contract.|
| ticketType | 1, 2, 3 | 1 is FTX, 2 is CNEO, 3 is CGAS. |
| wishNumber | number | 1 ~ 39.|
| wishNumber | number | 1 ~ 39.|
| wishNumber | number | 1 ~ 39.|
| wishNumber | number | 1 ~ 39.|
| wishNumber | number | 1 ~ 39.|
| referralHash? | string | Who gets 5% of ticket price. |

`drawLottery(args[])`

| Arg | type | Description
|--- |--- |--- |
| casterHash | string | Who gets 5% of ticket sales of the game. |


`verifyLotteryTicket(args[])`

| Arg | type | Description
|--- |--- |--- |
| casterHash | string | Who gets 5% of the ticket price. |
| ticketNo? | number | if not ticket no set, it verifies using the latest verification height. |


#### Helper methods:

`claimLotteryWinningTicket(ticketNo?)`

`getLotteryHeight()`

`getLotteryEntryHeight()`

`getLotteryVerificationHeight()`

`getLotteryWinnerHeight()`

`getLotteryClaimHeight()`

`getLotteryTicket(ticketNo)`

`getLotteryResult(gameNo)`

`getLotteryWinner(height)`

`getLotteryPool(currency, gameNo)`

`getLotteryUserBalance(ownerHash, currency)`

`getTimeLeft()`

`getLotteryCurrentJackpots()`

`getLotteryParticipation()`

`getLotteryVerification()`

`getLotteryClaim()`

#### Admin only:
`launchLottery()`

