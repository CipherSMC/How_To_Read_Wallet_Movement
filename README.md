# How to read wallet movements

**Author:** 0xNox (@0xNoxxx)  
**Date:** August 12, 2026  
**Source:** [https://x.com/0xNoxxx/status/2087541333120405841](https://x.com/0xNoxxx/status/2087541333120405841)

![Cover - How to read wallet movements](https://pbs.twimg.com/media/HPhlnI3WwAAp2VF.jpg)

A practical guide for anyone who sees onchain alerts and does not know what to do with them.

I have been watching onchain data for years. Whale flows, funding rates, unlock schedules, exchange balances. It's one of the few parts of this market you can verify for yourself. Once a transaction happens, it's there for everyone to see.

I post those movements every day. Cold wallet to hot wallet. Bridge outflows. Treasury transfers. And the most common reply I get is a fair one. What does that actually mean?

So this is the answer. Not a thread, a proper walkthrough. By the end you will be able to look at any alert on your timeline, including mine, and work out whether it should change what you are doing with your position.

## Why onchain data comes first

You cannot see a company's bank account. But you can see a crypto project's treasury, the team's wallet, and a whale's full position. The blockchain is a public ledger. Every transfer is recorded and nobody can delete it.

That's why onchain data can often give you a heads-up before the news does.

An exchange empties its wallets before it collapses. A team sends tokens to an exchange before it sells. A whale piles up stablecoins before it buys.

By the time the headline hits, the move may already be underway. The transfer is often the earlier signal.

But there is a trap here. Onchain data does not tell you what will happen. It only tells you what has happened. That's the distinction you need to keep in mind when reading onchain data.

## First, whose address is it?

Most alerts you see, including mine, involve one of six kinds of address. Once you understand these, most wallet alerts become much easier to read.

One thing to clear up first, because it trips up almost everyone. Hot and cold describe whether a wallet is connected to the internet. They do not describe who owns it. An exchange has a cold wallet and a hot wallet. A whale has a cold wallet and a hot wallet. Saying "hot wallet" without saying whose is meaningless.

![Not every wallet means the same thing](https://pbs.twimg.com/media/HPhi5FIWgAAke-i.jpg)

- **Exchange cold wallet.** The venue's own offline reserve. It moves rarely and when it does, it moves in size.
- **Exchange hot wallet.** The working account. It absorbs deposits and pays out withdrawals. It is busy all day.
- **Deposit address.** A unique address the exchange hands to each user, on each chain. This is where real inflow appears. It is the single most useful address type in this whole business.
- **Fresh wallet.** An address created days ago with almost no history. When size lands in a fresh wallet, something new is starting. A new position, an OTC settlement, or a stack being split up.
- **Side wallet.** An address with no label in Arkham that sits between two known entities. Teams and whales use these as a hop so the origin is harder to read. A side wallet is not proof of anything by itself. It is a reason to keep clicking.
- **Known entity.** A treasury, a market maker, a fund or a custody provider. These are already tagged, so you know who you are looking at, but the label alone doesn't tell you much. A treasury is usually a multisig and money leaves it for a reason. Tokens arriving at Wintermute or GSR are often there to be quoted on both sides of the book, not sold. And a custody address like Fireblocks has dozens of clients behind it, so you can see the movement without ever knowing whose decision it was.

When you see an alert, the first question is never how much. It is who.

## Second, which way is it going?

I look at the direction first, not the size. A large transfer means very little if you don't know where it's coming from or where it's going. Almost every alert on your timeline is one of the seven flows below, and three of them are not news at all.

![Read the direction before the amount](https://pbs.twimg.com/media/HPhjA2uXIAAN3dM.jpg)

- **Private wallet to a deposit address.** This is the part of the flow I pay the most attention to. New supply is arriving at a venue where it can be sold. A deposit doesn't mean a sale is coming, but tokens generally need to reach a venue before they can be sold on its order book.
- **Deposit address to exchange hot wallet.** This is the sweep. The exchange is collecting your deposit into its working account. The same coins have already been counted once. Counting them again inflates a number that never changed.
- **Exchange hot wallet to exchange cold wallet.** Housekeeping. The venue is parking what it does not need day to day. Not bullish, not bearish.
- **Exchange cold wallet to exchange hot wallet.** A refill of the working account. It usually means withdrawals are being processed, not that the exchange is preparing to sell anything.
- **Exchange hot wallet to a fresh wallet.** A withdrawal. Someone pulled size off the venue and into a brand new address. That is worth following, because a fresh wallet has no history to explain it yet.
- **Side wallet to anywhere.** An unlabelled hop. Somebody added a step to make the origin harder to read. Keep clicking until you reach an address you can name.
- **Any wallet to a bridge.** The money is changing chain. Not a sale. But nobody pays bridge fees and waits for a plan that lasts an afternoon.

Two more worth knowing, even though they show up less often in alerts. A wallet moving into a DeFi contract for staking or lending is keeping the token, not exiting it. And a wallet splitting into several fresh addresses is usually dividing a stack rather than preparing to sell.

## What actually happens inside an exchange

This part deserves its own section, because most bad onchain takes are born here.

When you deposit to an exchange, your coins do not land in one big pot. They pass through a chain of addresses.

![What happens inside an exchange](https://pbs.twimg.com/media/HPhjSX1XoAAY9-s.jpg)

1. The exchange gives you a deposit address. It is unique to you, on that chain, and it exists only to receive your funds. This is where your coins arrive.
2. Then the exchange sweeps that deposit address into its hot wallet. The hot wallet is the working account. It pays withdrawals and keeps the operation liquid.
3. Finally, whatever the exchange does not need day to day gets pushed into its cold wallet, offline, for safety.

This distinction matters when you're reading exchange alerts.

The first transfer into the deposit address is the part that matters. Real inflow is measured when coins hit the deposit address. That is a decision made by an outsider. That is new supply arriving.

The sweep is not new money. Deposit address to hot wallet is the same coins moving one step deeper inside the same company. If you count both, you have doubled a number that did not change.

Cold storage moves are housekeeping. An exchange shifting funds from its hot wallet to its cold wallet is not bearish or bullish. It is a treasurer doing their job.

The same logic runs in reverse on the way out. Cold wallet to hot wallet at an exchange is usually just refilling the working account before withdrawals. It is not the exchange preparing to dump.

So when a bot posts an alert, look at which leg of this chain it caught. Half the alerts on your timeline are internal plumbing dressed up as news.

## What a bridge actually does

Chains do not talk to each other. A token on Ethereum cannot simply walk over to Solana. A bridge is the machinery that makes the crossing possible.

The mechanism is simple. The token gets locked or burned on one side. A matching amount gets minted on the other side. So the token does not really travel. It stays where it was and a representation of it is born somewhere else.

Two things follow from that.

- A bridge transfer is not a sale. Only the address and the chain change. Reporting a bridge outflow as selling pressure is one of the most common mistakes on crypto Twitter.
- A bridge transfer shows intent. Bridging is slow, it costs money and it is a hassle. Nobody moves millions to another chain for a plan that lasts an afternoon. So when you see size crossing, the real question is what is waiting on the other side.

The answer is usually one of three things. An expected airdrop. Better yield. The start of a new narrative.

And if a chain keeps taking in more money than it sends out, week after week, that tells you more than any single wallet ever will.

## Third, how big is it really?

A dollar figure on its own means nothing. Four hundred thousand dollars is a disaster for one token and background noise for another.

Convert it into ratios. There are three worth knowing, and they tell you whether the market can absorb the move or not.

- **Share of circulating supply.** Around 1% is worth a look. 5% is serious. Above 10% and you have a story.
- **Share of 24 hour volume.** If a deposit is the size of half a day's trading, the market cannot absorb it without moving.
- **Against orderbook depth.** This is the strictest measure. Find out how much selling it takes to push the price down 2%. If the incoming amount is a multiple of that, the impact is real.

This is why I always publish the ratio alongside the amount. A raw dollar number will mislead you almost every time.

## Fourth, could it be nothing?

The fastest way to waste your time onchain is to treat noise as a signal. These are the six traps I check for before I act on anything.

- **Exchange reshuffles.** Exchanges move funds between their own wallets constantly. That unlabelled address receiving 200 million dollars might just be Binance's new cold wallet.
- **Custody movement.** Funds leaving Fireblocks tell you nothing about whose decision it was. Many clients share the same rails.
- **OTC deals.** A large share of big transfers are already agreed trades. The buyer exists. No selling pressure ever reaches the orderbook. If anything it means demand showed up.
- **Market maker inflow.** Projects send tokens to market makers so they can quote both sides. Reading that as a dump is wrong.
- **Double counting.** The same ten million dollars moving from A to B to C fires three alerts. It looks like thirty million dollars of activity. It is one pot of money. Exchange sweeps are the classic version of this.
- **Wrong labels.** Labels are added by people. If an address was tagged as a team wallet once by mistake, that mistake gets copied around for years.

So before you let an alert change your position, ask the boring question. Could there be a dull explanation for this? If the answer is yes, you have no trade.

## How to check any of this yourself

You do not have to take my word for it, or anyone else's. It is all open data.

- **Block explorers.** Etherscan, Solscan, BscScan, Arbiscan. Paste an address and you see its entire history.
- **Labels and flows.** Arkham and Nansen put names on addresses so you can see who is behind them. The free tiers cover most of what you need.
- **Portfolio view.** DeBank and Zapper show everything a wallet holds across every chain on one screen.
- **Bridge tracking.** LayerZero Scan, Wormhole Scan and the deBridge explorer let you find where a crossing landed on the other side.
- **Unlocks.** Token Unlocks and Cryptorank tell you whether a transfer lines up with a vesting event.

One habit is worth more than all of these tools. When you see a transfer, do not stop there. Click the receiving address and look at what it does next. The story continues there.

## Let's read one together

Say you see this on your timeline.

> 4.2 million dollars of TOKEN left the project treasury, passed through an unlabelled side wallet, and landed on a Binance deposit address.

Here is how it breaks down.

- **Who:** the treasury, so an insider. The side wallet in the middle is not a second party. It is the same money taking a hop.
- **Direction:** the final leg is a deposit address. That is real inflow, the leg that counts.
- **Count:** once. Three transfers fired, but 4.2 million moved, not 12.6 million.
- **Size:** measure 4.2 million against circulating supply and against daily volume.
- **Timing:** check whether an unlock or an announcement is close.

Your conclusion sounds like this. Nothing has been sold yet. But insider supply is now sitting where it can be sold, and someone took the trouble to route it through an extra address first. If the exchange balance keeps climbing, the signal builds. If the coins come back out to a fresh wallet, it was probably an OTC settlement.

Notice that I'm not making a price prediction here. I'm just laying out the conditions I'd watch next.

## So what do you actually do with it?

Reading the chain is only half the work. Here is how a read turns into a decision, or into no decision at all.

- An alert is not an entry. It is one input. A deposit that arrives while funding is already negative and open interest is climbing means something. The same deposit on a quiet day means very little.
- Wait for the confirming leg. Cold to hot on its own tells you nothing. Cold to hot, then a deposit address, then exchange balance rising over two days, is a different picture. Most of the time the confirming leg never comes, and that is the useful part.
- Let the ratio set the size, not the headline. If the flow is a fraction of daily volume, it does not deserve a change in position size. If it is a multiple of orderbook depth, it deserves your full attention.
- Decide in advance what would prove you wrong. If you read a deposit as sell pressure, then coins leaving again to a fresh wallet is your answer. It was an OTC settlement. Close the idea and move on.
- Respect the clock. Deposited coins can sit for weeks. Onchain gives you direction and pressure, not timing. Anyone who tells you it gives timing is selling something.

The honest summary is that most alerts should change nothing about what you are doing. The goal isn't to find a trade every time you see an alert. Most of the time, the better decision is to do nothing.

## The takeaway

I don't treat onchain data as a prediction tool. It shows me what happened and what is happening, not what someone is going to do next.

I wouldn't act on a single transfer. I want to see the direction, size, wallet history and timing all make sense together. Until they do, an alert is information, not a reason to touch your position.

It comes down to four questions. Whose wallet, which direction, how big against supply and volume, and what has that address done before.

Answer those four before you size a position and you are reading the chain. Skip them and you are trading on a screenshot.

## Who writes this

I trade and analyse onchain data, mostly whale flows, exchange balances, funding, open interest and unlock schedules. I have been doing it for years. I use charts too, but I spend a lot of my time looking at the data behind the price.

I started posting this work publicly three months ago. Since then it has reached over 8 million impressions and more than 10,000 people have followed along. I think the main reason people stuck around is that I don't just post the transfer. I explain why I think it matters.

I am not a caller. I do not post buy and sell signals. I share what the chain shows, how I read it, and where I am wrong.

If you want the alerts as they happen, follow me on X at [@0xNoxxx](https://x.com/0xNoxxx).

For longer breakdowns and live flow tracking, the Telegram channel is here: [t.me/oxnoxflow](https://t.me/oxnoxflow)
