# dhandle

Because fair and portable web3 social handles matter!

## Motivation


## Scope


## Model

- What is a name? /[a-zA-Z0-9_-]{3,64}/
- Reserve it by staking ETH on the contract
- We get a non-transferable NFT that represents our handle
- Challenge? call bid() with at least 2x the current ETH stake or 2x the current bid
- Current owner can match() with the challenged amount to keep the name by sending the current stake, and the challenger gets their ETH back
- From last bid, the contract will close the auction after 30 days, this will reset after each contract interaction (bid or match)
- The new owner can claim() ownership after the auction is closed, and the current owner gets his stake back.