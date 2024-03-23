
## Stake and Bake - unity.beta.v1 - Thirdweb x Earn Alliance integration [[play here](https://snb-kappa2.vercel.app/)]


Stake and Bake is a cross-chain DeFi game rewarding chain loyalty and chain-agnostic behaviour simultaneously.

Join the first cross-chain DeFi game playable across 5 networks. Claim your free $BUDS and in-game NFTs now to be eligible for exciting rewards on mainnet launch. Are you 'degen' enough to design a winning strategy to maximize your $BUDS? Compete with our community of degens in a game where players get rewarded for their loyalty to their network, or by seizing hard-earned $BUDS from other chains! Play across Ethereum, Arbitrum, Avalanche, Polygon, and Binance Chain.

## How Thirdweb tools serve the needs of Stake and Bake:

***Thirdweb Embedded Wallets:*** The game uses Thirdweb's account factory to create smart wallets for users.

***Thirdweb Unity SDK:*** This is used for interacting with our game contracts, to sign messages, and for listening to on-chain events using the built-in RPC. 

It is crucial to the functioning of our game as the core game functions for our on-chain game are called using the Unity SDK. These include:

- On-chain Raids (Cross-chain and on connected chain)
- Staking (cross-chain and on connected chain)
- Minting Game Assets
- Faucet Claims

***Thirdweb Connect:*** We have used the connect wallet modal for users to connect to the game via multiple wallet providers. The login options for email, social, or guest wallets are particularly useful to onboard non-native crypto users.

We use the following wallet actions: connect/disconnect wallet, contract interactions, view balance, switch networks etc.

## Use of Earn Alliance Events API

For this implementation, we have created a challenge on Earn Alliance which requires players to raid farms across two separate networks to earn rewards. The players may choose to raid a farm across Arbitrum, Avalanche, BSC, Ethereum and Polygon. 

*[Click here to view the challenge](https://www.earnalliance.com/challenges/stake-and-bake/raid-a-farm-to-seize-buds)*

In order to enable this challenge and monitor user activity, the game uses a separate nodeJS backend to listen to game contract events and leverages the EarnAlliance REST API to update the status of challenges.

