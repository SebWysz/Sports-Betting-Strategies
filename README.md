# Sports-Betting-Strategies
I write about what I have learned while creating edge against sportsbooks, and thoughts about the strategies.

## Storytime (Skip if you don't care)

I learned about sports-betting arbitrage from a friend in college. He said he could give me ~$200 if I just let him use my sports betting account for BetMGM. The sign up bonus at the time was a no-sweat bet of $1500. If you lose, they give you the money back as a bonus bet. A bonus bet can be viewed as extra leverage, you can wager this money, but you only keep the earnings (Normal: $100 to win $200 total would be $100 bonus bet to win $100 total). Anyways, I thought this was insane! Free money? From a casino of all things? I thought the house always won...

So I asked him, how do you do it? One word: Arbitrage. I had heard of the term before, but I thought arbitrage was out of my reach -- reserved for the HFT firms and computer automated trading companies. I was interested in making some money, so I'm thankful he was willing to let me in on his secrets. Thank God becasue he was taking a 60% cut if you just gave him the account.

He said he does it with a program named OddsJam (https://oddsjam.com/), which he paid for, and it gave him the lines to bet on. This was epic. I now had access to the same resource he used so I could make my own money.

There are other websites that offer the same service, but OddsJam is the one I ended up using. It is a relatively expensive service, but I had no issues with the platform and the support is awesome.

## How I Began

First, I started by leveraging the sign up offers of the different books available in Illinois. If you have no accounts open yet, ideally you partner up with a friend who does have an account open so you can arbitrage the sign up offers of bonus bets. I personally had a DraftKings account open already, so I used that to convert FanDuel's bonus bets. From here, you just use whichever lines and books that have the best conversion rate out of the books you have accounts with. On average a bonus bet can be converted into real money at a 70% rate. Once you have some books open and a solid bankroll (either from the sign up offers or your own money; ~$500, but still possible with lower amounts), you can hit normal arbitrage opportunities that appear.

## Promotion Conversion Math
### Bonus Bets
Bonus bets are extra leverage you can put on a line, so to earn a high conversion rate, usually the bonus bet line would be +200 or more while the hedge would be the opposite at around -200 or less.

Assume we have two opposite lines that are +300 and -350 (bonus bet lines do not have to be an arbitrage for the conversion, although it would give a better rate sometimes). Converted to decimal, +300 odds becomes $\frac{300}{100} + 1 = 4$, and -350 becomes $\frac{100}{350} + 1= 1.2857$

Then say we have a $50 bonus bet, so

$50 \cdot 4 = 200$

But since we don't include the $50 initial bet, we have a payout of $150. Then the hedge bet is calculated as

$\frac{150}{1.2857} = 116.6679$

But we would round to at least the nearest dollar, but usually the nearest 5 or 10 so the sportsbooks are less likely to catch on.

This calculation leaves us with the two outcomes (assume we hedge with $115$, the bonus bet line winning, in which case we earn a profit of

$150-115 = 35$

Or the hedge line winning, where we earn a profit of

$115 \cdot 1.2857 - 115 = 32.8555$

Then we take the lower profit (or average if you want) and say that is our conversion amount, $32.8555/50 = 0.657$. So this situation has a conversion rate of 65%.


### No Sweat
A no-sweat bet is one that if the bet loses, you get a portion (usually 100%) of your bet back as a bonus bet. This can be leveraged to make some money.

Let's use the same lines of +300 and -350, and say the no-sweat bet is for a maximum of $50. Similar rules apply, but now we factor in the bonus bet money we get if that line loses, simplified to 70% of the bonus bet amount.

So if no-sweat line wins, it earns

$50 \cdot 4 - 50 = 150$

Then we calculate a hedge bet as (Where $50 \cdot 0.7$ is the amount we win from the given bonus bet if no-sweat line loses) 

$\frac{50 \cdot 4 + 50 - 50 \cdot 0.7}{1.2857} = 128.33$

Say we round this up to $130, then our profit if the no-sweat line wins is

$50\cdot 4 - 50 - 130 = 20$

And if the hedge bet wins

$130 \cdot 1.2857 - 130 - 50 + 50\cdot 0.7 = 22.14$

Guaranteed profit of at least 20 dollars, so we would call this a 40% ( $\frac{20}{50}=0.4$ ) conversion. A general good rate of conversion for these is around 50% imo.


### Profit Boost
Profit boosts are promotions that increase your profit by the percent it says (Ex: 25%, 50%, 100%). Therefore it increases the line's decimal value, so it becomes a good arbitrage because of the changed payout.

Let's use the same lines again of +300 and -350, and say the profit boost is 75% with a max bet of $50. We calculate the modified line's payout and then simply calculate as an arbitrage.

So we calculate the 75% profit boost on the +300 line from the decimal value, but only the profit of 3x gets increased by 75%,

$(4 - 1) \cdot 1.75 + 1 = 6.25$

Converting that back into American odds, it is +525, which is the same as $300 \cdot 1.75 = 525$.

Now we have an arbitrage, so we calculate our hedge bet since we know that the max bet of the profit boost is $50.

$\frac{50 \cdot 6.25}{1.2857} = 243.06$

Rounding this to $245, our profit if the profit boost line wins is calculated as

$50 \cdot 6.25 - 50 - 245 = 17.5$

And our profit if the hedge wins is

$245 \cdot 1.2857 - 245 - 50 = 20$

So we call this a 35% ($\frac{17.5}{50} = 0.35$) conversion.

## Arbitrage Math
An arbitrage is possible if we look at two opposite lines and their American Odds sum is positive (if it's negative you lose money, and if it's zero, you neither gain nor lose if bet sizes are correct). This is probably the only nice thing about American odds in my opinion.

Ex: A +300 and -350 line sums to -50, so not an arbitrage, but a +350 and a -300 line sums to +50, which is an arbitrage opportunity

Say we do have the +350 and -300 lines. To calculate the percent arbitrage, we get the decimal odds first.

$350 / 100 + 1 = 4.5$

$100 / 300 + 1 = 1.33$

Then given an input for a maximum bet, say at most $300 on one line, we calculate the other side of the arbitrage as

$\frac{300 \cdot 1.33}{4.5} = 88.66$

Which we will round to $90. Then our profit if the $300 bet wins is

$300 \cdot 1.33 - 300 - 90 = 9$

And if the $90 line wins,

$90 \cdot 4.5 - 90 - 300 = 15$

The asymmetry in profit is due to the rounding. We would then call this a 2.3% arbitrage ($9 / (300 + 90) = 0.023$).

That's really all there is to it. As long as you properly size your wager, there is no risk involved with this strategy.

## +EV Betting (and why I didn't do it)

+EV stands for positive expected value. It's a term in statistics that, when wagered on infinitely, you are expected to make money because you have an edge.

On OddsJam, they calculate an expected value via a type of average on all the sportsbook's lines to get an expected probability of the event happening. Then if one line deviates significantly (the wager pays more than you should expect for the implied odds), it is a +EV bet that you should take. The software then calculates a bet size for you using how much percent edge you have over the market and the Kelly criterion (typically quarter Kelly) which is *very* important for this strategy. (The Kelly criterion is important because otherwise you could bankrupt your portfolio with a higher probability -- take a quarter of that, and you lessen both the risk and reward... and the chance of bankruptcy)

However, there are some concerns I have with this strategy especially in the world of sportsbooks, in which I chose not to partake in this strategy.

First, nobody really knows the true probability of a certain sports event occuring. If one book deviates significantly, there are two options. The book is smart, and knows something the other books don't, or the book made a mistake. When you're only taking one side of the spread, how should you know which is which? It's a game of imperfect information which can be lucrative, but I liked taking the assured gain, especially when it was so frequent.

There is also a history of sportsbook lines and certain books are known to be "sharper" (better at setting true odds) than others. For example two of the sharpest sportsbooks I've heard of are Pinny and Circa Sports. They accept all bets and any size instead of limiting winning bettors. The books then use the information of when a sharp (smart) bettor places a bet to adjust their true odds. Their odds then lay where the money goes. Some people only average the sharp books' lines to calculate an implied probability which does better. I just never really got into it.

## How to track your cash
You need to track your cash. Without some sort of ledger, cash might be disappearing right under your nose. My way of doing this was tracking it on OddsJam manually when I placed a bet, and also using Pikkit to automatically scrape betting accounts and accumulate the bets I have placed.

With Pikkit, I am assured that I have been placing the correct bets. Since a lot of lines are very similar, this gives me peace of mind that I pressed the right buttons outside of OddsJam. OddsJam also provides a ways to sync your sportsbooks, but I wanted both a manual and automatic to assure my intentions matched my actions.

## Limits & End of an Era :/
If you talk to any sharp
