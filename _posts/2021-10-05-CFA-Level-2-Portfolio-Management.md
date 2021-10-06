---
toc: true
layout: post
description: CFA Level 2 Portfolio Management summary
categories: [markdown]
title: CFA Level 2 Portfolio Management
---
# CFA Level 2 Portfolio Management

## LOS 43.a: Explain the creation / redemption process of ETFs and the function of authorized participants.

Unlike open-end mutual funds, ETFs are traded on secondary markets.

The ETF issuer designates authorized participants (APs). APs are permitted to create additional shares, or redeem existing shares, for a service fee payable to the ETF manager.

The in-kind creation / redemption process serves three purposes:

1.   Lower cost
2.   Tax efficiency
3.   Keeping market prices in line with NAV

This implies that ETFs should trade within a price band of the NAV, known as the arbitrage gap.

Investor -> ETF (상장) -> 추종하려는 Index (결국 ETF 가격은 Index 가격에 따라 움직임)

Authorized Participants (AP)라는 역할 존재

상장이니까 가격 변동성 존재 (NAV에서 가격이 멀어질 수 있음) -> AP가 조절 by 증자, 감자

장점

-   Lower Cost - 증자, 감자는 AP가 해주니 ETF Manager는 신경쓰지 않음
-   Tax Efficiency: ETF의 증자 / 감자는 비과세
-   NAV와 가격 같게 유지 -> 그렇지 않으면 arbitrage gap 발생 가능

## LOS 43.b: Describe hoe ETFs are traded in secondary markets.

In the United States, the National Security Clearing Corporation (NSCC) guarantees the performance of parties to a trade on an exchange. The Depository Trust Company (DTC), a subsidiary of NSCC, transfers the securities from the account of the seller's broker to the account for buyer's broker at the end of the two-day settlement period. Market makers, due to their special significance, and due to the time required by the creation / redemption process, are afforded up to six days to settle their trades.

ETF는 주식처럼 상장되어 거래, NSCC가 성과 보증하고 DTC가 거래 소관 (2영업일 내에 거래 처리)

AP는 증자 / 감자 거래 처리를 6영업일 안에 처리

## LOS 43.c: Describe sources of tracking error for ETFs.

Tracking difference is the divergence between an ETF's return (based on its NAV) and the return on the tracked index. Tracking error is the annualized standard deviation of the daily tracking difference. Tracking error does not indicate whether the ETF under- or outperformed the index.

ETFs generally underperform the benchmark by their expense ratio.

Sources of tracking error include the following:

1.   Fees and expense
2.   Sampling and optimization
3.   Depository receipts (DRs) - due to time zone differences in capturing price data
4.   Index changes
5.   Regulatory and tax requirements
6.   Fund accounting practices
7.   Asset manager operations

Tracking difference: BM과 ETF return의 차이

Tracking error는 ETF가 Index보다 성과가 좋다 나쁘다 개념이 아님 - 잘 복제했느냐 개념

ETF가 BM보다 성과가 보통 낮은 이유 -> Fees, Sampling, DR, Index 변화, 규제 변화, Fund accounting, asset manager operation

## LOS 43.d: Describe factors affecting ETF bit-ask spreads.

The primary factors affecting ETF spread are the liquidity and the market structure of the underlying securities.

-   Spreads on fixed-income ETFs tends to be larger than hose for large-cap equity ETFs.
-   The spreads are narrower during the overlapping time period when both markets are open.
-   Specialized ETFs, such as those that track commodities, volatility futures, or small-cap stocks, tend to have wider spreads.
-   Thinly-traded ETFs, regardless of the liquidity of the underlying, also command a higher spread.

Maximum spread = creation (redemption) fees plus other trading costs + spread of the underlying securities + risk premium for carrying the trade until close of trading + AP's normal profit margin - discount based on probability of offsetting the trade in secondary market

Bid-Ask spread가 영향을 미치는 주요 요인 - 해당 시장의 유동성, underlying security

채권 ETF spread가 더 큼, specialized ETF spread가 더 큼

Maximum spread = Creation fee + spread (기초자산) + risk premium + AP's margin - discount (유통시장에서 거래되어 offsetting 될 수 있는 비용)

## LOS 43.e: Describe sources of ETF premiums and discounts to NAV.

The NAV of an ETF is generally its fair value.

ETF premium (discount) % = (ETF price - NAV per share) / NAV per share

-   Timing differences - ETFs on foreign securities may experience gaps between the time the ETF is traded and the time when the underlying trades in a foreign market.
-   Stale pricing - Infrequently traded ETFs may reflect noncurrent prices and, therefore, their value may differ from NAV.

ETF prices may be more informative than NAV or iNAV when 1) the market for the underlying is closed, 2) underlying securities are highly volatile or illiquid, or 3) there is a time lag between the pricing of the ETF and the pricing of underlying.

ETF는 일반적으로 fair value에 거래됨 - 거래소가 NAV를 공시

ETF premium = (ETF price - NAV price) / NAV price

premium이나 discount 발생 이유 - timing difference, stale pricing

하지만 NAV보다 ETF price가 더 의미있을 때도 있음 - 장전, 기초자산이 너무 변동성이 심할 때 등

## LOS 43.f: Describe costs of owning an ETF.

ETF costs include management fees and trading costs.

Trading costs include brokerage or commission fees and bid-ask spreads.

For shorter holding periods, trading cost dominates the cost of ETF ownership. Conversely, long-term investors are likely to seek out ETFs with low management fees.

Management fee + trading costs -> 경쟁이 치열하고 + passive라서 fee수준은 낮은 편

trading costs는 거래할 때만 발생 -> 보유기간이 길 수록 거래비요으이 비중은 감소 -> 장기투자자는 운용보수가 낮은 ETF 선호

## LOS 43.g: Describe types of ETF risk.

### Counterparty risk

Exchange-traded notes (ETNs), for example, have high counterparty risk. In the case of an ETN, an issuer (typically a bank) issues unsecured debt obligations that promise to pay the return on an index less management fees (just like a regular ETF).

The concern here is that the bank may default, resulting in losses for the ETN investor.

### Settlement risk

ETFs using OTC derivative contracts as part of their strategy expose investors to the settlement risk of such contracts.

### Security lending

Like mutual funds, ETFs may lend their securities to short sellers for a fee.

### Fund closures

### Expectation-related risk

The outcomes may differ from investors' expectations

The compounding effects of leveraged ETFs make them unsuitable for buy-and-hold investors with investment horizons exceeding one month.

Counterparty risk, settlement risk, security lending, fund closures, expectation-related risk (기대와 다른 효과)

## LOS 43.h: Identify and describe portfolio uses of ETFs.

Due to their low costs, tax efficiency, and wide variety, ETFs are suitable for numerous portfolio strategies.

### Efficient portfolio management

1.   Portfolio liquidity management
2.   Portfolio rebalancing
3.   Portfolio completion
4.   Transition management

### Asset class exposure management

Allow a manager to implement a variety of strategies suitable for their clients.

1.   Core exposure to an asset class or sub-asset class
2.   Tactical strategies

### Active investing

Newer varieties of ETFs with an active component have gained traction, especially for fixed income.

1.   Factor (smart beta) ETFs
2.   Risk management
3.   Alternatively weighted ETFs
4.   Discretionary active ETFs
5.   Dynamic asset allocation and multi-asset strategies

Efficient Portfolio management 활용 - liquidity, rebalancing, completion, transition

assets class exposure management 활용 - core exposure, tactical strategy

active investing - factor ETF, risk management, alternatively weighted ETF, Discretionary active ETF, Dynamic asset allocation -> ETF는 유동성이 있으니 자유자재로 active하게 활용해서 $\alpha$추구

## LOS 44.a: Describe arbitrage pricing theory (APT), including its underlying assumption and its relation to multifactor models.

Arbitrage pricing theory (APT) was developed as an alternative to the capital asset pricing model. However, unlike CAPM, APT does not identify the specific risk factors (or even the number of factors).

### Assumptions of arbitrage pricing theory (APT)

1.   Unsystematic risk can be diversified away in a portfolio
2.   Returns are generated using a factor model
3.   No arbitrage opportunities exist

### The APT eqaution

$$
\\E(R_{P}) = R_{F} + \beta_{P, 1}(\lambda_{1}) + \beta_{P, 2}(\lambda_{2}) + ... +  \beta_{P, k}(\lambda_{k})
$$

$\lambda_{j}$ equals the risk premium for a portfolio (called a pure factor portfolio) with factor sensitivity equal to 1 to factor j and factor sensitivities of zero for the remaining factors.

Unlike the CAPM, the APT does not require that one of the risk factors is the market portfolio. This is a major advantage of the arbitrage pricing model.

Arbitrage pricing model -> CAPM 왜 한 개인지 의문이 발생 -> 수익률에 영향을 주는 게 더 많지 않을까라는 의문에서 개발 (베타 말고 다른 요인 찾기)

가정

1.   비체계적 위험은 분산 가능
2.   Return은 Factor model로 측정 가능
3.   Arbitrage 기회 없음

이름이 왜? - 위 2번 가정을 모두가 쓰면, 모두가 같은 $E(r)$을 계산 -> mispricing이 생겨도 금방 수정됨 -> arbitrage 기회 없음

Factor Portfolio = 다른 Factor는 다 0으로 가정, Factor 1개만 1로 측정 -> 그래서 그 factor가 얼마나 영향을 주는지를 측정하기 ㅜ이함

장점 - Factor를 다중 분석할 수 있음

단점 - 어느 Factor를 써야하지? 통계적으로 맞다 하여도 쌩뚱맞은 변수를 쓰면 무슨 소용이지?

## LOS 43.b: Define arbitrage opportunity and determine whether an arbitrage opportunity exists.

The APT assumes there are no market imperfections preventing investors from exploiting arbitrage opportunities.

Over-valued는 short, 그 돈으로 under-valued 매수 -> 그 차이가 이익

## LOS 43.c: Calculate the expected return on an asset given an asset's factor sensitivities and the factor risk premiums.

## LOS 43.d: Describe and compare macroeconomic factor models, fundamental factor models, and statistical factor models.

A multifactor model assumes asset returns are driven by more than one factor. There are three general classifications of multifactor models: 1) macroeconomic factor models, 2) fundamental factor models, and 3) statistical factor models.

1.   Macroeconomic factor models assume that asset returns are explained by surprises (or shocks) in macroeconomic risk factors. Factors surprises are defined as the difference between the realized value of the factor and its consensus predicted value.
2.   Fundamental factor models assume asset returns are explained by multiple firm-specific factors.
3.   Statistical factor models use statistical methods to explain asset returns. Two primary types of statistical factor models are used: factor analysis and principal component models. The major weakness is that the statistical factors do not lend themselves well to economic interpretation. Therefore, statistical factors are mystery factors.

### Macroeconomic factor models

$$
\\R_{i} = E_{R_{i}} + b_{i1}F_{GDP} + b_{i2}F_{QS} + \epsilon_{i}
\\R_{i} = \text{return for Asset i}
\\E_{R_{i}} = \text{expected return for Asset i (in the absence of any surprises)}
\\F_{FDP} = \text{surprise in the GDP rate}
\\F_{QS} = \text{surprise in the credit quality spread (BB-rated bond yield - Treasury bond yield)}
\\b_{i1} = \text{GDP surprise sensitivity of Asset i}
\\b_{i2} = \text{credit quality spread surprise sensitivity of Asset i}
\\\epsilon_{i} = \text{firm-specific surprise (unrelated to the two macro factors)}
$$

-   Each "F" is a factor surprise, the difference between the predicted value of the factor and the realized value.
-   The firm-specific surprise captures the part of the return that can't be explained by the model.

Be careful to interpret the signs properly.

#### Priced risk factors

A risk does not affect many assets can usually be diversified away in a portfolio and will not be priced by the market.

The factors in our example model, GDP and credit quality spread shocks, are systematic risk factors, meaning that they will affect even well-diversified portfolios.

#### Factor sensitivities

In a macroeconomic multifactor model, asset returns are a function of unexpected surprises to systematic factors, and different assets have different factor sensitivities.

The factor sensitivities of the model can be estimated by regressing historical asset returns on the corresponding historical macroeconomic factors.

### Fundamental factor models

$$
\\R_{i} = a_{i} + b_{i1}F_{P/E} + b_{i2}F_{SIZE} + \epsilon_{i}
\\R_{i} = \text{return for stock i}
\\F_{P/E} = \text{return associated with the P/E factor}
\\F_{SIZE} = \text{return associated with the SIZE (market capitalization) factor}
\\a_{i} = \text{intercept}
\\b_{i1} = \text{standardized sensitivity of stock i to the P/E factor}
\\b_{i2} = \text{standardized sensitivity of stock i to the SIZE factor}
\\\epsilon_{i} = \text{portion of asset i return not explained by the factor model}
$$

Standardized sensitivities ($b_{i1}$ and $b_{i2}$). Sensitivities in most fundamental factor models are not regression slopes. Instead, the fundamental factor sensitivities are standardized attributes.
$$
\\b_{i1} = \frac{(P/E)_{i} - \bar{P/E}}{\sigma_{P/E}}
$$
Factor returns ($F_{P/E}$ and $F_{SIZE}$). The fundamental factors are rates of return associated with each factor. The dependent variable is the set of returns for all stocks and the independent variables are the standardized sensitivities.

### The macroeconomic factor model vs. the fundamental factor model

-   Sensitivities - The standardized sensitivities in the fundamental factor model are calculated directly from the attribute data-they are not estimated. The macroeconomic model, in which the sensitivities are regression slope estimates.
-   Interpretation of factors - The macroeconomic factors are surprises in the macroeconomic variables. In contrast, the fundamental factors are rates of return associated with each factor and are estimated using multiple regression.
-   Intercept term - The intercept in the macroeconomic factor model equals the stock's expected return. In contrast, the intercept of a fundamental factor model with standardized sensitivities has no economic interpretation.

![image-20211005210656567](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211005210656567.png)

![image-20211005210702810](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211005210702810.png)

![image-20211005210710178](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211005210710178.png)

![image-20211005210715799](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211005210715799.png)

## LOS 44.e: Explain sources of active risk and interpret tracking risk and the information ratio.

Active return equals the differences in returns between a managed portfolio and its benchmark:
$$
\\\operatorname{Active return} = R_{P} - R_{B}
$$
Active risk (also known as tracking error or tracking risk) is defined as the standard deviation of the active return:
$$
\\\operatorname{Active risk} = \operatorname{tracking error} = \sigma_{R_{P} - R_{B}}
$$

### The Information Ratio

Active return alone is insufficient for measuring an investment manager's performance over a series of measurement periods.

To demonstrate a manager's consistency in generating active return, we use the information ratio, which standardizes average active return by dividing it by its standard deviation.
$$
\\\operatorname{IR} = \frac{\bar{R_{P}} - \bar{R_{B}}}{\sigma_{R_{P} - R_{B}}}
$$
The higher the IR, the more active return the manager earned per unit of active risk.

![image-20211005211415233](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211005211415233.png)

## LOS 44.f: Describe uses of multifactor models and interpret the output of analyses based on multifactor models.

$$
\\\operatorname{active return} = R_{P} - R_{B}
\\\operatorname{factor return} = \sum_{i = 1}^{k}{(\beta_{pi} - \beta_{bi}) * \lambda_{i}}
\\\operatorname{security selection return} = \operatorname{active return} - \operatorname{factor return}
\\\beta_{pi} = \text{factor sensitivity for the ith factor in the active portfolio}
\\\beta_{bi} = \text{factor sensitivity for the ith factor in the benchmark portfolio}
\\\lambda_{i} = \text{factor risk premium for factor i}
$$

### Risk attribution

$$
\\\operatorname{active risk} = \operatorname{tracking error} = \sigma_{(R_{P} - R_{B})}
$$

The active risk of a portfolio can be separated into two components:

1.   Active factor risk
2.   Active specific risk

$$
\\\operatorname{active risk squared} = \operatorname{active factor risk}^{2} + \operatorname{active specific risk}^{2}
\\\operatorname{active factor risk}^{2} = \operatorname{active risk squared} - \operatorname{active specific risk}^{2}
$$

![image-20211006144910041](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006144910041.png)

### Uses of multifactor models

#### Passive management

Managers seeking  to track a benchmark can construct a tracking portfolio. Tracking portfolios have a deliberately designed set of factor exposures.

#### Active management

Active managers use factor models to make specific bets on desired factors while hedging (or remaining neutral) on other factors. A factor portfolio is a portfolio that has been constructed to have sensitivity of one to just one risk factor and sensitivities of zero to the remaining factors. Factor portfolios are particularly useful for speculation or hedging purposes.

#### Rules-based or algorithmic active management (alternative indices)

These strategies use rules to mechanically tilt factor exposures when constructing portfolios.

### Carhart Model

$$
\\E(R) = R_{F} + \beta_{1}\operatorname{RMRF} + \beta_{2}\operatorname{SMB} + \beta_{3}\operatorname{HML} + \beta_{4}\operatorname{WML}
\\\operatorname{RMRF} = \text{return on value-weighted equity index - the risk-free rate}
\\\operatorname{SMB} = \text{average return on small cap stocks - average return on large cap stocks}
\\\operatorname{HML} = \text{average return on high book-to-market stocks - average return on low book-to-market stocks}
\\\operatorname{WML} = \text{average returns on past winners - average returns on past losers}
$$

![image-20211006145212417](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006145212417.png)

## LOS 44.g: Describe the potential benefits for investors in considering multiple risk dimensions when modeling asset returns.

Under the CAPM framework, investors choose a combination of the market portfolio and the risk-free asset depending on their risk tolerance. By including more risk factors, multifactor models enable investors to zero in on risks that the investor has a comparative advantage in bearing and avoid the risks that the investor is incapable of absorbing.

![image-20211006145246246](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006145246246.png)

## LOS 45.a: Explain the use of value at risk (VaR) in measuring portfolio risk.

Value at risk (VaR) measures downside risk of a portfolio. It has three components: the loss size, the probability (of a loss greater than or equal to the specified loss size), and a time frame.

VaR can also be expressed in percentage terms so that for a portfolio, we could state that the 5% monthly VaR is 3%, meaning that 5% of the time the monthly portfolio value will fall by as least 3%.

![image-20211006153109480](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006153109480.png)

![image-20211006153117871](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006153117871.png)

![image-20211006153122956](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006153122956.png)

## LOS 45.b: Compare the parametric (variance-covariance), historical simulation, and Monte Carlo simulation methods for estimating VaR.

## LOS 45.c: Estimate and interpret VaR under the parametric, historical simulation, and Monte Carlo simulation methods.

### Parametric method

One method of estimating VaR is the parametric or vairance-covariance method. Assuming normally allows us to estimate the risk of the portfolio based only on the means, variances, and covariances (or correlations) of the various risk factors. (skewness and kurtosis)

Assuming normality, we can use the portfolio variance formula to estimate the mean and variance of portfolio returns.
$$
\\\sigma_{Portfolio}^{2} = W_{A}^{2}\sigma_{A}^{2} + W_{B}^{2}\sigma_{B}^{2} + 2W_{A}W_{B}Cov_{AB}
$$
lookback period - The important point is that the parametric estimates we use should be those we expect over the period for which we are estimating the VaR.

The parametric method is relatively simple to apply under the assumption of normally distributed returns. The length of the lookback period will affect the parameter estimates. In cases where normality cannot be reasonably assumed, such as when the portfolio contains options, the parametric method has limited usefulness.

![image-20211006153135086](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006153135086.png)

### Historical simulation method

The historical simulation method of estimating VaR is based on the actual periodic changes in risk factors over a lookback period.

Under the historical simulation method, no adjustment are made for the difference between the results for the lookback period and the results over a longer prior period.

One positive aspect of the historical simulation method is that we do not need the assumption of normality, or any other distributional assumption, to estimate VaR.

VaR estimates will depend on the lookback period and, as with any forecasts, will vary with the characteristics of the sample data used.

![image-20211006153141597](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006153141597.png)

### Monte Carlo simulation

A third method of VaR estimation is Monte Carlo simulation. Monte Carlo simulation is based on an assumed probability distribution for each risk factor.

This procedure is repeated thousands of times. As with the other methods, the data used and the assumptions about the distributions of the risk factors will have significant effects on the estimated VaR.

![image-20211006153148238](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006153148238.png)

## LOS 45.d: Describe advantages and limitations of VaR.

### Advantages of VaR

-   The concept of VaR is simple and easy to explain.
-   VaR allows the risk of different portfolios, asset classes, or trading operations to be compared to gain a sense of relative riskiness.
-   VaR can be used for performance evaluation.
-   When allocating capital to various trading units, a firm's risk managers can also look at the allocation of VaR, and optimize the allocation of capital given the firm's determination of the maximum VaR.
-   Global banking regulators accept VaR as a measure of financial risk.
-   Reliability of VaR as a measure of risk can be verified by backtesting.

### Limitations of VaR

-   VaR estimation requires many choices (loss percentage, lookback period, distribution assumptions, and parameter estimates) and can be very significantly affected by these choices.
-   The assumption of normality leads to underestimates of downside (tail) risk because actual returns distributions frequently have "fatter tails" than a normal distribution. Although the assumption of normality is not a requirement of VaR, it is almost always used, especially with the parametric method.
-   Liquidity often falls significantly when asset prices fall.
-   It is well known that correlations increases, or spike, during periods of financial stress. VaR measures based on normal levels of correlation.
-   While VaR is a single number that can be used to quantify risk, as with any summary measure, many aspects of risk are not quantified or included.
-   VaR focuses only on downside risk and extreme negative outcomes. Including consideration of right-hand tail values will give a better understanding of the risk-return trade-off.

![image-20211006153747046](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006153747046.png)

![image-20211006153754436](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211006153754436.png)

## LOS 45.e: Describe extensions of VaR.

### Conditional VaR

Another measure based on Var is the conditional VaR (CVaR). The CVaR is the expected loss, given that the loss is equal to or greater than the VaR. For this reason, the CVaR is also referred to as the expected tail loss or expected shortfall.

When the VaR is estimated using the historical simulation method or Monte Carlo simulation, we have all the losses greater than the VaR loss, so it is straightforward to take the average of these to get the CVaR. With the parametric method, we don't know the magnitude of losses greater than the VaR, so calculating the expected loss in the left-hand tail is mathematically complex.

