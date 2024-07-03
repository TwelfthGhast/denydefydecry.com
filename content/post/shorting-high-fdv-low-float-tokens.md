+++
title = 'Shorting high FDV, low float tokens :)'
date = 2024-07-03T21:07:46+10:00
draft = false
summary="Is shorting high FDV, low float tokens free money? That's probably a yes. A really badly written summary and a trade idea"
+++
# Shorting high FDV, low float tokens :)

## The basics

_What does FDV mean?_

FDV, or Fully Diluted Valuation refers to the total marketcap of a token assuming all tokens are in circulation.
It can be calculated using the token price multiplied by the total supply of the token.
A longer explanation can be found [here](https://www.coingecko.com/learn/what-is-fully-diluted-valuation-fdv-in-crypto).

_What does low float mean?_

A _low float_ token, is a token that has a small circulating supply, relative to its final circulating supply.

## The thesis
Low float tokens that have a high FDV are likely priced high relative to their "true" value and their prices should drop as the circulating supply increases. The ideal token to short is a high FDV token with a known unlock schedule while also being relatively cheap to maintain a short position in.

## The risks

### Reduction of future supply.

Tokens can be burned / rendered inaccessible and thus effectively reducing the FDV of a token. One example is when the founder of the Jupiter aggregator on Solana [proposed a 30% burn](https://x.com/weremeow/status/1803453096661590363) of total supply, resulting in an almost 10% spike in the price of JUP, with action absent in any of the other major tokens.

![JUP Chart](/images/jup_20240620.png)
![SOL Chart](/images/sol_20240620.png)

### Short squeeze AKA Getting blown up

You don't want to be GameStop'd and blown out of your shorts; make sure you have sufficient margin and keep an eye out on potential squeezed coins that you might want to open new positions on. A good indicator to watch for is open interest on the coin relative to the current circulating market cap. See WLD below.

## Some historical examples

### LDO

Lido is a governance token for a [LST](https://www.coingecko.com/learn/what-is-liquid-staking-liquid-staked-derivatives-you-need-to-know) protocol. Not just "a" protocol but *the* protocol, being the largest liquid staking protocol for ethereum.

Yet despite circulating marketcap increasing by over 10x from 2022 to 2024, price has remained stagnant. That being said, price hasn't really decreased so you probably wouldn't have made a profit shorting unless you had a good entry.

Here are your LDO charts:
![LDO Circulating Market Cap](/images/ldo_circ_mc.png)
![LDO Price](/images/ldo_price.png)

That being said, what if you hedged your short LDO position with a long ETH position? This looks quite promising :)
![ETH Price](/images/eth_price.png)

Now as an exercise to the reader:
- Is long ETH a good hedge for short LDO? Why or why not?
- Coingecko provides summary data available for download - crunch the numbers yourself

### WLD

Worldcoin is a "proof of humanity" coin by our controversial Sam Altman (associated with OpenAI and YCombinator). With an incredibly low float, WLD ran up to over $10 at one point - bringing the fully diluted value of WLD at over $100 billion dollars. Incredibly overvalued! Great calls by @defisquared: [first post](https://x.com/DefiSquared/status/1762059166477168824), [second post](https://x.com/DefiSquared/status/1790075349373694174)

![WLD Price](/images/wld_price.png)

## A trade idea (As of July 2024)

We want to short a high FDV, low float coin. The trade idea I'm proposing is short JTO; Jito being a governance protocol on Solana is currently around $2.40 a token, with only around 1/8 of it's 1 billion supply circulating at the moment. [Token Unlocks](https://token.unlocks.app/jito-governance-token) expects around 1.6 million JTO tokens being released as emissions per week from subsidising liquidity providers for pools on Orca/Kamino Finance/other on Solana. Additionally, the one year cliff finishes on the 7th of December, 2024 when 135 million tokens unlock.

### Funding costs

Currently funding rates are very slightly positive on Binance Futures as crypto market is still slightly bullish with 19 million JTO in open interest, so you are getting paid to short. Onchain borrowing is about 1-2% APY; but this is much more margin inefficient.

### Expected Value

How much are governance tokens really worth? Depends on who you ask - but the best example is probably the LDO/stETH ratio; how much LDO is trading relative to how much ETH is locked up in Lido. As of July, the FDV of LDO is around 1.8 billion (and 90% of tokens in circulation), with total locked ETH around 32 billion so the governance token is trading at a 1:18 ratio with TVL. Jito currently has a 1.7 billion TVL, so you would expect a more realistic FDV to be around 100 million - this means we can expect the short leg to drop 90% in value in a good scenario. However, I **believe** JTO has a longer vesting period than LDO so the short leg won't be that profitable.

### Hedging

JTO is a Solana native token and should have some beta to Solana. So to hedge a short JTO position, we would want to long Solana; Solana also loses value due to inflation, so make sure to hedge with either staked Solana or an LST. The difficult question is how would you hedge the betas correctly...