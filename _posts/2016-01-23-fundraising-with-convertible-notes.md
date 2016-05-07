---
layout: 	post
date: 		2016-01-23 12:00:00
title:		"Convertible notes are mispriced"
cover:      /images/caution.jpg
categories: [fundraising, startups]
---

I met an investor today who suggested we consider raising money with a convertible note. He said it's super fast and we don't have to get into a valuation discussion. When I expressed my hesitation, he told me I was crazy and then proceeded to tell me how proud he was to have recently invested in a high profile seed-stage company with an uncapped convertible note. This is nuts. Let me explain why.

Convertible notes seem to be all the rage these days amongst startup founders and (strangely) investors and it has really been bothering me because it means the "entrepreneurial" community is no better than pre-crisis bankers, and actually much worse. At least bankers tried to price the risk.

### Bonds
Bonds are the fundamental building block of our society. Governments implement monetary policy through regular issuances of bonds, companies finance their everyday operations through bonds and the general public gobbles these up in their pensions and savings. 

Bonds work very simply: An investor gives a company 100 dollars today to get (100 + X) back at a set time in the future, The size of X depends on the probability of default of the company. In other words, will the company still be operational, and if so will they have the funds to pay back (100 + X)? 

> **BOND MECHANICS**  
> t0: Investor ----- $100------->  Company  
> t1: Investor <----$100 + X----  Company   

### Credit Risk
Now, if the "Company" is two people and a 10-slide deck, the chance of default is immense (95% of startups fail, right?) so that amount for X is ridiculously high. 
X represents the "credit risk" of a company or, in other words, the risk that the company goes bust in the year and the lender doesn't get their money back. Credit risk has a simple formula:

> X = PD*(1-RR) where,  
> PD = Probability of Default  
> R = the Recovery Rate (amount recovered at default)  

Unlike a government bond, when a startup goes bust, investors write if off and lose everything. There are no fixed assets to sell. The Recovery Rate = 0.
As discussed above, PD = 95%. So our X is 95%. 
This means that the company should theoretically be offering an interest rate of 99% on their convertible note. Double the investment!

### Return
So now let's imagine the company was worth $1mn at seed stage and does really well and grows exponentially. Exponential growth is e^x where x is the number of years (e ~ 2.7). Startup investments are typically sized to give 18months of runway with the assumption that the fund-raising process starts 6months prior, at 12months. 
So at 12 months, when the founders start looking to raise more money, the company is worth 2.7 times its original value ($1mn). To the founders this looks great, right? No.
The new, series A, investors are looking at a company worth $2.7, *but with a $2mn liability* to pay in 6 months, right about when the new Series A funding will arrive. In reality then, the company is worth only $0.7mn - less than at the seed stage!
This also means that most of the new investment will go towards paying the old investors and not towards growing the business. This is great for the old investors (who just doubled their money) but awful for the new investors, so they simply won't invest (unless they are even more clueless than the angels and caught up in the hype). As a founder, you are trapped between a rock and a hard place and despite your exponential growth, your company is un-investable and ultimately not worth much.

This is why early stage debt investment doesn't make sense and doesn't happen. Yes, banks don't lend money to startups, for their own good. Bet you didn't see that coming.

### Options
Let's put bonds aside for a second and talk about call options. Simply, a Call Option gives the buyer the right to buy shares in 18 months at today's price. So if the share price goes up, the buyer exercises his rights and gets shares at a discount, if shares go down, the buyer doesn't exercise and writes-off the price of the option. The economics look like this:

> **OPTION MECHANICS**  
> t0: Investor ------Option Price---->  Company  
> t1: Investor <----$0 or (equity)----  Company   

Options aren't free though and a simple pricing formula is the volatility (standard deviation) of the stock price over the last year times the square root of the number of years:

> Option Price = vol. * sqrt(Y)  

Given that your fledgling company went from 0 to $1mn in a matter of minutes, the volatility is very close to 100%. So for a 1-year option, the price of that option is also about 100% of the share price, let's call it 99%. 

If the option was 3% of the stock price you would write it off (barring a 97% drop in the shares) but if you are paying close to 100% for an option, you will always choose the equity because you would rather get something back as an investor (even if it is less than what it cost you).

### Convertible Bonds
Convertible bonds (CB) are simply a bond + an option packaged together. In other words, on day 1 the investor buys a bond ($100), but then also pays the company the option price ($100*99%). So after a year, the investor either gets the bond return (from above) or the investment converts to equity.

> **CONVERTIBLE BOND MECHANICS**  
> t0: Investor -------$100 + $99------------>  Company   
> t1: Investor <--($100 + $95) or (equity)---  Company   

But we know (from above) that the bond payout option is not really a possibility for a startup:  

- If the company's stock price has fallen below it's seed stage valuation, things are really bad and the startup won't have any money to pay back the bond, no recovery assets and the option will expire worthless. So in reality the CB returns $0.
- If the company's stock price has soared, it converts to equity. Yay!

> **CONVERTIBLE BOND MECHANICS for STARTUPS**    
> t0: Investor ------$100 + $99------>  Company   
> t1: Investor <--($0) or (equity)----  Company   

So what was the point of all that financial structuring if the investor just gets equity in the end anyways? What happened here? We priced the risk!

But most convertibles don't price the risk. If we look at the famous SAFE Note, investors set the interest rate at something a large corporate like IBM would pay (5%) and the company sells the  option for free. So our mechanics looks like this:

> **STARTUP CONVERTIBLE NOTE**    
> t0: Investor -----------$100-------------->  Company   
> t1: Investor <--($100 + $5) or (equity)----  Company   

Look familiar? That look appetizing now, win-win for an investor and the startup gets some cash. Just because we ignored the risk and didn't price though, doesn't mean it went away. (Remember what happened with mortgage-backed securities anyone?)

But the company still won't have the money to pay the investors $105 if the share price has fallen in a year (ie. it is running out of runway with no business model). So really, the true mechanics look like this:

> **STARTUP CONVERTIBLE NOTE in REALITY**    
> t0: Investor -------$100----------->  Company   
> t1: Investor <----$0 or (equity)----  Company   

Hey, that looks just like the economics of an option!

### Misaligned Interests
So why not just sell investors an option? The company sells employees options. The termsheet is even simpler than the supposedly "cheap and fast" convertible that people advertise. Well debt investors get some nice benefits over equity investors and option investors get no rights (no votes, no dividends). Debt investors get paid back before equity ones, and depending on the terms, can sometimes force a company that looks unlikely to pay back its debt to wind up and hand over the remaining cash.

The bottom line is that different types of investors have different agendas:    
- Debt investors are interested in getting paid back the money they have lent to the company, plus interest.  
- Equity investors want to have a vote on management and are interested in the long-term financial health of the business.  
- Option investors are only interested in seeing the share price go up beyond what they paid to turn a profit (speculation). This is regardless of whether or not the share price reflects the true value of the company.  

As a founder, your interests are only aligned with equity investors. Debt holders are trying to take your money away, and option investors are trying to unsustainably inflate your share price.

If you are setting sail on a dangerous voyage, you want to recruit crew who are going to be with you in the galley, in the doldrums and share their bread with you to stave off starvation. You don't want funders who are only interested in their cargo coming back to shore or merchants betting on how much cargo you will return with.

Sure, you can impose caps and other clever tricks in your convertible note to prevent some of this behavior, but only up to a point. And if you are putting a cap then aren't you implicitly setting a valuation anyways?

If there is one thing I learned from a decade in banking, it is that:

> Financial innovation and the mis-pricing of risk is at its highest the moments before a market crash.


