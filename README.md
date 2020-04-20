# ***STOCK ANALYSIS***
---

# Contents
## 1. [Need to invest and investments](#need-to-invest)
## 2. [Trading Stocks](trading-stocks)
## 3. [Options Trading](options-trading)

---

# Need to invest and investments

In a nutshell, investment is important inorder to shield ourselves from inflation and generate wealth.

We can invest in any of the following asset classes :
1. Fixed income instruments
2. Equity
3. Real estate
4. Commodities (precious metals)

# Trading Stocks

# Options Trading

## Moneyness of an Option :
> Moneyness of an option is a classification method which classifies each option strike based on how much money a trader is
likely to make if he were to exercise his option contract today.  
There are 3 broad classifications –
1. In the Money (ITM)
2. At the Money (ATM)
3. Out of the Money (OTM)

If the intrinsic value is a non zero number, then the
option strike is considered ‘In the money’. If the intrinsic value is a zero the option
strike is called ‘Out of the money’. The strike which is closest to the Spot price is
called ‘At the money’.  In general, ITM
options are always more expensive compared to OTM options.  

## Option Greeks :
> The premium of the option depends on certain forces called as the ‘OptionGreeks’. Crudely put, some Option Greeks tends to increase the premium, whilesome try to reduce the premium. Though all these factors work as independent agents, yet they are all intervened with one another. A formula called the ‘Black & Scholes Option Pricing Formula’ employs these forces and translates the forces into a number, which is the premium of the option.  

These are the Option Greeks:  
1. Delta – Measures the rate of change of options premium based on the directional
movement of the underlying
2. Gamma – Rate of change of delta itself
3. Vega – Rate of change of premium based on change in volatility
4. Theta – Measures the impact on premium based on time left for expiry

### Delta of an Option:
> The Delta measures how an options value changes with respect to the change in the underlying. *i.e;* Delta is the rate of change of *Premium* with respect to *Underlying*.  
The delta is a number which varies –
1. Between 0 and 1 for a call option, some traders prefer to use the 0 to 100 scale. So
the delta value of 0.55 on 0 to 1 scale is equivalent to 55 on the 0 to 100 scale.  
2. Between -1 and 0 (-100 to 0) for a put option. So the delta value of -0.4 on the -1 to 0
scale is equivalent to -40 on the -100 to 0 scale.  

**Note-** 
- The delta value cannot be greater than 1. If that is the case, the change in value of premium will be more than that of underlying stock which is codswallop. Option is derived from its underlying and it can never move faster than the underlying itself.
- The delta value cannot be less than 0 as there is a chance that premium becomes negative because of negative delta.

The delta changes with changes in the value of spot. Hence delta is a variable and not really a fixed entity. Therefore if an option has a delta of 0.4, the value is likely to change with the change in the value of the underlying. It's relation can represented through the following graph :-   
![Delta vs Moneyness](https://zerodha.com/varsity/wp-content/uploads/2015/06/Image-1_Delta-vs-Spot1.png)

Note the following points about the above graph (written with respect to call option but similar observations can be made for put option) -
- The delta value increases as spot value increases
- Delta doesn't change much when monyness is deep OTM or OTM ( similarily with deep ITM and ITM).
- Delta hits 0.5 at ATM.

We can conclude the following (written for call options)-
- Deep OTM options tends to put on an impressive percentage however for this to happen the spot has to move by a large value.
> The change in premium is proportional to change in underlying (by a factor of delta). The premiums are low for OTM options hence a meaningful change in underlying can give massive yields of premium in terms of percentages.
- The slightly OTM option which usually has a delta value of say 0.2 or 0.3 is more sensitive to changes in the underlying. For any meaningful change in the underlying the percentage change in the slightly OTM options is very impressive.
> The delta is higher than deep OTM options hence less risk and more returns. The risk is lower because if the spot price decreases the delta value remains almost same (curve is flatter and change is low) and the returns are more because if spot price increases the delta value increases rapidly (acceleration stage). In a vague manner, we are talking about f"(x) and not f'(x). *We can say that the premium vs spot price curve looks like an exponential curve here.* Note that the premiums are higher in case of OTM options when compared to deep OTM ones.
- ATM options are more sensitive to changes in the spot when compared to OTM options. Now because the ATM’s delta is high the underlying need not really move by a large value. Even if the underlying moves by a small value the option premium changes. However buying ATM options are more expensive when compared to OTM options.
> The percentage yields are lower because the premium also increased rapidly when compared to OTM options.
- In terms of the absolute change in the number of points, the deep ITM option scores over the slightly ITM option. However in terms of percentage change it is the other way round. Clearly ITM options are more sensitive to the changes in the underlying but certainly most expensive.
> The risk is lowest in ITM options. When delta is 1 (deep ITM), buying a deep ITM option is as good as buying the underlying itself. This is because whatever is the change in the underlying, the deep ITM option will experience the same change. Deep ITM option moves in line with the underlying, this means you can substitute a deep ITM option to a futures contract (lesser margin though).

The above can be summarised as follows - 
The price is 2210 and the expectation is a 30 point change in the underlying (which means we are expecting spot price to hit
2240). We will also assume there is plenty of time to expiry; hence time is not really a concern.  
| Moneyness | Strike | Delta | Old Premium | Change in Premium | New Premium | % Change |  
| --- | --- | --- | --- | --- | --- | --- |
| Deep OTM  |  2400  | 0.05  |   Rs.3/-    |   30* 0.05 = 1.5  | 3+1.5 = 4.5 |   50%    |
|Slightly OTM| 2275| 0.3| Rs.7/-| 30*0.3 = 9| 7 +9 = 16| 129%|
|ATM| 2210| 0.5| Rs.12/-| 30*0.5 = 15| 12+15 = 27| 125%|
|Slightly ITM| 2200| 0.7| Rs.22/-| 30*0.7 = 21| 22+21 = 43| 95.45%|
|Deep ITM| 2150| 1| Rs.75/-| 30*1 = 30| 75 + 30 =105| 40%|
