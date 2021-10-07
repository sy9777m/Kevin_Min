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

-   VaR을 넘어선 손실에 대한 측정 - VaR을 넘어갔다고 가정
-   Historical & Monte Carlo - 계산이 어려움
-   Parametric - 계산 쉬움

### Incremental VaR (IVaR)

-   Security가 추가(감소) 될 때 증분 VaR

### Marginal VaR (MVaR)

We can interpret it as the change in VaR for a 1% increase in the security's weight. Thus, both the MBaR and IVaR can be used to estimate the change in VaR that will result from a change in the weight of a single security.

-   Portfolio 안에 weight 들이 미치는 VaR 측정 for 위험관리
-   직관적 이해 - Before & After = IVaR, 시점전날 전력투구 과목 고르기 = MVaR

## Ex ante tracking error (relative VaR)

Ex ante tracking error measures the VaR of the difference between the return on a portfolio and the return on its manager's benchmark portfolio.

Benchmark와 Portfolio의 차이 VaR

## LOS 45.f: Describe sensitivity risk measures and scenario risk measures and compare these measures to VaR.

### Sensitivity analysis

Risk assessment using sensitivity analysis focuses on the effect on portfolio value given a small change in one risk factor. Portfolio risk can be better understood and more effectively managed. Unlike VaR, it does not invlove any prediction of the probability of losses of any specific amount.

-   민감도 분석, 각 Factor의 영향력 분석
-   specific 확률을 제공하진 않음

### Scenario analysis

Scenario analysis provides an estimate of the effect on portfolio value of a set of changes of significant magnitude in multiple risk factors.

-   각 factor들의 가정들 set -> 결과값 -> 분석
-   Historical scenario - 역사적 기반
-   Hypothetical scenario - 가상값
-   Stress testing - 극단값

#### Historical scenario

A historical scenario approach uses a set of changes in risk factors that have actually occurred in the past.

#### Hypothetical scenario

With a hypothetical scenario approach, any set of changes in risk factors can be used, not just one that has happened in the past.

#### Stress test

Stress tests examine the effect on value (or solvency) of a scenario of extreme risk-factor changes.

## LOS 45.g: Demonstrate how equity, fixed-income, and options exposure measures may be used in measuring and managing market risk and volatility risk.

The risk factors used to measure the risks of equities, fixed-income securities, and options are all different. For equities, the most often used risk factor is beta.
$$
\\E(R_{i}) = R_{f} + Beta_{i}[E(R_MKT) - R_{f}]
$$
For fixed-income securities and portfolios, duration provides an estimate of how market values are affected by changes in interest rates (yield to maturity). For larger changes in interest rates, including the effects of convexity on fixed-income security values improves estimates of the sentisivity of the values of fixed-icnome securities to changes in interest rates.
$$
\\\operatorname{Change in price} = -Duration(\Delta{Y}) + \frac{1}{2}Convexity(\Delta{Y})^2
$$
Several risk factors affect the values of options positions. Delta is an estimate of the sensitivity of options values to changes in the value of the underlying asset.

-   Delta, Gamma, Vega

1.   Equity - Beta
     -   CAPM
2.   Fixed Income
     -   Duration, Convexity
3.   Option
     -   Delta, Gamma, Vega

### LOS 45.h: Describe the use of sensitivity risk measures and scenario risk measures.

Sensitivity risk measures can inform a portfolio manager about a portfolio's exposure to various risk factors to facilitate risk management. Of course, eliminating all risk is not the goal.

Factor sensitivities can be used to estimate the effects of small changes in risk factors for these securities.

Pricing models can be quite accurate when all of the relevant characteristics of a security are specified.

Scenario analysis is often performed as if the scenario changes were instantaneous.

In reverse stress testing, the first step is to identify a portfolio's largest risk exposures. The question then becomes how likely such scenarios are. Using scenario analysis in this way can be beneficial in helping risk managers identify the vulnerabilities of a portfolio and perhaps mitigate the risk exposures identified.

Sensitivity risk measures - manager에게 risk들을 선택할 수 있게 활용 (베팅, 헷징)

Scenario analysis - 상황변화에 대해 즉각적인 대응을 가능하게 함

Reverse stress testing - testing을 통해 원인 찾기 -> 실제 일어날 수 있을지 여부 검토

## LOS 45.i: Describe advantages and limitations of sensitivity risk measures and scenario risk measures.

VaR, sensitivity analysis, and scenario analysis complement each other, and a risk manager should not rely on only one of these measures.

The problem with using duration as the risk measure is that the yield volatility of one portfolio may be quite different from the yield volatility of the other.

VaR = %, loss 제공

Sensitivity analysis = 각 factor 별 영향 제공, %는 제공 안함

Scenario analysis = 각 factor set 별 영향 제공, %는 제공 안함

서로 모두 보완역할

## LOS 45.j: Describe risk measures used by banks, asset managers, pension funds, and insurers.

For each type of organization, differences among firms will result in differences in the risk measures used.

Banks typically use sensitivity measures (duration of held-to-maturity securities and foreign exchange risk exposure), scenario analysis and stress testing (for their full balance sheets), leverage risk measures, and VaR (especially for trading securities). Banks also estimate risk from asset-liability mismatches, estimate VaR for economic capital, and disaggregate risk by both geographic location and business unit type.

Traditional (long-only) asset managers typically focus on relative risk measures unless their goal is an absolute return target. A risk measure more specific to asset management is active share: the difference between the weight of a security in the portfolio and its weight in the benchmark.

Ex-post tracking error (backward looking) and ex ante tracking error (forward looking) measures provide different information. Ex-post tracking error is used for performance attribution and to assess manager skill over prior periods. Traditional asset managers mostly use ex ante tracking error for risk estimation. Managers with an absolute return target may use VaR instead.

For hedge funds, the risk measures used depend, to some extent, on the strategy employed.

Hedge funds with significantly non-normal returns distributions use a risk measure referred to as maximum drawdown: the largest decrease in value over prior periods of a specific length.

Defined benefit pension funds calculate the difference between the present value of their assets (often market values) and the present value of their estimated future liabilitieis (payments to retirees and heirs). A risk measure used by pension funds is surplus-at-risk, a VaR for plan assets minum liabilities.

Insurance companies are often subject to significant regulation of their products and their investment portfolios (reserves). Property and casualty insurers sell auto, home, boat, liability, and health insurance. Insurance risks are reduced by pruchasing reinsurance (from another insurance company) and by geographical diversification.

P&C insurers use sensitivities of their exposures to market risk factors in their investment portfolios for risk management.

The insurance risk of life insurers is more highly correlated with the market risk exposures of their investment portfolios than it is for P&C insurers. The present value of these liabilities are quite sensitive to the discount factors used.

Bank - 보수적, 다 사용한다고 보면 됨

Traditional (long-only) manager - 보통 relatvie risk measure (benchmark랑 비교)

-   ex-post tracking error - 성과평가 용으로 활용
-   ex-ante trackign error - risk 미리 측정으로 활용
-   absolute return은 VaR 활용

Hedge fund - 전략마다 다 위험지표 다름

-   정규분포가 아닌 경우 -> Maximum drawdown 사용

DB pension fund

-   P(A) - P(L) = surplus -> 위험관리 대상

Insurance

-   손보사
    -   risk가 market과 상대적으로 연관이 적음
    -   관리대상 - 보험료 + 운용수익으로 총 비용 cover가 가능한지 여부
-   생보사
    -   life time annuity 판매 -> 부채로 계상
    -   시장 할인율이 어떠냐에 다라 부채의 변동성이 심해지는 risk가 market과 상대적으로 연관이 높음

## LOS 45.k: Explain contraints used in managing market risks, including risk budgeting, position limits, scenario limits, and stop-loss limits.

Risk limits that are often imposed include following.

Risk budgeting refers to a risk management process that first determines the acceptable total risk for an organization, and then allocates that risk to different activities, strategies, or asset classes as appropriate.

Position limits are one way to limit risk because they ensure some minimum level of diversification by limiting risk exposures. For example, position limit may be imposed on allocations to individual securities within an asset class, asset classes such as equities or high-yield bonds, investments in a single country, securities in a single currency or the differences between long and short positions for a hedge fund manager.

Scenario limits are limits on expected loss for a given scenario.

Stop-loss limits require that a risk exposure be reduced if losses exceed a specified amount over a certain period of time.

1.   Risk budgeting - firm의 risk를 정하고 -> allocation to 각 부서
2.   Position limit - 특정행위 금지 (투기채, 특정주식, 특정국가 등)
3.   Scenario limit - 주어진 시나리오에서의 제한행위
4.   Stop-loss limit - 손실이 특정 범위를 넘어서면 risk exposure 감소시킴

## LOS 45.l: Explain how risk measures may be used in capital allocation decisions.

Capital aalocation decisions refer to how the capital of a firm is used to fund its various business units or activities, analogous to asset aalocation for a portfolio manager. Risk management, however, requires that the risk exposure for each use of firm capital be considered.

One way to introduce risk exposures to various activities into the capital allocation decision is to limit the overall risk of all the activities.

risk 무시하고 return 극대화를 위한 allocation? -> risk exposure를 고려해야 함 ex) VaR 배분

## LOS 46.a: Explain the notion that to affect market values, economic factors must affect one or more of the following: 1) default-free interest rates across maturities, 2) the timing and / or magnitude of expected cash flows, and 3) risk premiums.

The value of any asset can be computed as the present value of its expected future cash flows discounted at an appropriate risk-adjusted discount rate.

Components of the discount rate are:

1.   Real risk-free discount rate (R)
2.   Expected inflation($\pi$)
3.   Risk premium reflecting the uncertainty about the cash flow (RP)

The value of an asset will change if either the cash flow forecasts change or any of the components of the discount rate changes.

Value = Cash flow / (1 + Discount Rate)

-   Value는 CF가 변해도, 할인율이 변해도 변할 수 있음

Discount rate = real rate + inflation + risk premium

-   할인율 역시 자산이 변해도, Investor의 기대가 변해도 변할 수 있음

## LOS 46.b: Explain the role of expectations and changes in expectations in market valuation.

The value of an asset depends on 1) its expected future cash flows and 2) the discounted rate used to value those cash flows. As market participants receive new information, the timing and amounts of expected future cash flows are revised and valuations change as a result. The impact of new information will depend on its effect on current expectations.

기존의 expectation -> CF 추정 / 할인율 추정 -> 결과

그런데 새로운 정보가 유입되어서 CF와 할인율이 변한다면 -> 기존의 결과가 변함

## LOS 46.c: Explain the relationship between the long-term growth rate of the economy, the volatility of the growth rate, and the average level of real short-term interest rates.

The real risk-free rate of interest derives from the inter-temporal rate of substitution, which represents an investr's trade-off between real consumption now and real consumption in the future.
$$
\\\operatorname{inter-temporal\, rate\, of\, substitution} = m_{t} = \frac{\operatorname{marginal utility of consuming 1 unit in the future}}{\operatorname{marginal utility of current comsumption of 1 unit}} = \frac{u_{t}}{u_{0}}
$$
Investors always prefer current comsumption over future consumption ($u_{0}>u_{t}$) and $m_{t} < 1$ as a result.
$$
\\P_{0} = E(m_{t})
\\R = \frac{1 - P_{0}}{P_{0}} = \frac{1}{E(m_{t})} - 1
$$

-   The higher the utility investors attach for current consumption relative to future consumption, the higher the real rate.
-   Investor's marginal utility of consumption declines as wealth increases.
-   If investors expect higher incomes in the future, their expected marginal utility of future consumption is decreased relatvie to current consumption.
-   Investors increase their savings rate when expected returns ar high or when uncertainty about their future income increases.

Real risk-free rate -> inter-temporal rate of subsitution (현재의 소비 vs 미래의 소비)

Mt = 미래효용 / 현재효용

투자자는 항상 현재를 더 선호 -> Mt < 1

![image-20211007163653421](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211007163653421.png)

기억해야 할 것

-   현재가 더 중요한 투자자 -> 더 높은 real rate을 가짐
-   부가 증가하면 소비효용은 감소한다 -> 소비효용이 증가하면 부가 감소하는 것을 의미 (경기 수축)
-   미래 수입의 증가를 기대 -> 미래 현재효용이 감소
-   미래 불확실성이 증대, 기대 return이 증가 -> 투자자의 saving 증가

### Risky cash flows and risk premiums

The risk aversion of investors can be explained by the covariance of an investor's inter-temporal marginal rate of subsitution and expected on savings. Investors experience a large loss of utility for a loss in wealth as compared to a gain in utility for an equivalent gain in wealth. This property is called as risk-aversion.

An investor's absoulte risk-aversion declines with their wealth; wealther investors are less risk-averse and more willing to take risk relative to their poorer counterparts. However, the marginal utility of holding risky assets declines as an investor holds more risky assets in her portfolio.
$$
\\P_{0} = \frac{E(P_{1})}{1 + R} + cov(P_{1}, m_{1})
\\R = \text{the real risk-free rate}
$$
The covariance between the expected future price of the bond and the investor's inter-temporal rate of substitution can be viewed as a risk premium. For risk-averse investors, the covariance is negative; when the expected future price of the asset is high, the marginal utility of future consumption relative oto current consumption is low. Everything else constant, the lower current price($P_{0}$) increases expected return.

risk aversion

-   같은 gain loss에서 loss에 더 고통스러워하는 자
-   부자일수록 absolute risk aversion은 감소
-   부자일수록 less risk averse, willingness to take risk 가능성 증가
-   risky asset이 많을수록, risk asset의 한계효용은 감소

![image-20211007163853789](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211007163853789.png)

### GDP growth rates

If GDP growth is forecasted to be high, the utility of consumption in the future (when incomes will be high) will be low and the inter-temporal rate of substitution will fall; investors will save less, increase real interest rates. Therefore, real interest rates will be positively correlated with real GDP growth rates.

GDP growth rate이 높은 것으로 기대

-   미래소비 효용 감소, less save
-   자금이 귀해지고 real interest rate 증가
-   결국 real interest rate과 GDP 변동성은 상관계수가 positive 관계

## LOS 46.d: Explain how the phase of the business cycle affects policy and short-term interest rates, the slope of the term structure of interest rates, and the relative performance of bonds of differing maturities.

Nomial risk-free interest rates include a premium for expected inflation ($\pi$). However, actual inflation is uncertain.

For short-term risk-free securities, the uncertainty about inflation is negligible.
$$
\\r(\operatorname{short-term}) = R + \pi
\\r(\operatorname{long-term}) = R + \pi + \theta
$$
For longer term bonds, we add the risk premium for uncertainty about inflation, $\theta$.

Actual inflation을 고려하자 (nominal)

1.   Short-term = R + inflation
2.   Long-term = R + inflation + actual

### Taylor rule

Central banks are usually charged with setting policy rates so as to 1) maintain price stability and 2) achieve the maximum sustainable level of employment.
$$
\\r = R_{n} + \pi + 0.5(\pi - \pi^{*}) + 0.5(y - y^{*})
\\\pi^{*} = \text{central bank's target inflation rate}
\\y = \text{log of current level of output}
\\y^{*} = \text{log of central bank's target (sustainable) output}
$$

-   price stability를 유지하며, 고용수준 최대 달성목표
-   중앙은행의 정책 이자율

### Business cycle and slope of the yield curve

When the economy is in recession, policy rates tend to be low. Leads to higher longer-term rates. This results in a positively sloped yield curve. Conversely, expectations of a decline in GDP growth results in a negatively sloped (inverted) yield curve. For this reason, an inverted yield curve is often considered a predictor of future recessions.

A term spread is the difference between the yield on a longer-term bond yield and the yield on a short-term bond. Evidence suggests that normal term spread is positive so the yield curve is upward sloping.

-   recession -> policy rate은 low
-   경기침체 벗어나기 위해 GDP 기대 올리고 + inflation 적절히 관리
-   YC가 우상향 (positively sloped YC)
-   GDP 감소 trend -> negatively sloped YC
-   Inverted YC가 종종 경기침체의 signal로 관찰됨
-   Term spread = LT bond - ST bond
-   Nominal term이 + -> upward YC
-   +라는 것은 -도 존재한다는 것을 의미

## LOS 46.e: Describe the factors that affect yield spreads between non-inflation-adjusted and inflation-indexed bonds.

The difference between the yield of a non-inflation-indexed risk-free bond and the yield of an inflation-indexed risk-free bond of the same maturity is the break-even inflation rate (BEI).
$$
\\BEI = \operatorname{yield\, on\, non-inflation-indexed\, bond} - \operatorname{yield\, on\, inflation-indexed\, bond} = \pi + \theta
$$
BEI is composed of two elements: expected inflation ($\pi$) and a risk premium for uncertainty about actual inflation ($\theta$).

## LOs 46.f: Explain how the pahse of the business cycle affects credit spreads and the performance of credit-sensitive fixed-income instruments.

The required rate of return for bonds with credit risk includes an additional risk premium. This credit risk premium (credit spread) is the difference in yield between a credit risky bond and a default-free bond of the same maturity.
$$
\\\operatorname{required rate of return for credit risky bonds} = R + \pi + \theta + \gamma
\\\gamma = \text{additional risk premium for credit risk} = \text{credit spread}
$$
Creadit spreads tend to rise during times of economic downturns and fall during expansions.

When credit spreads narrows, credit risky bonds will outperform default-free bonds. Overall, lower rated bonds tend to benefit more then higher rated bonds from a narrowing of credit spreads (their yields fall more). Conversely, when credit spreads widen, higher rated bonds will outperform lower rated bonds on a relative basis (because their yields will rise less).

Credit RP = 같은 만기 credit risky bond - default free bond

required rate = r + inflation + risk premium + yield curve credit spread

economic downterm -> spread 증가

economic expansion -> spread 감소

경제 위축 -> default 증가 -> credit loss 증가

bond 성과 -> spread가 좁아질 때 -> lower rate > higher rate

spread가 넓어질 때 -> lower rate < higher rate

## LOS 46.g: Explain how the characteristics of the markets for a company's products affect the company's credit quality.

Spreads differ among sectors and over time. Differences in credit spreads are primarily due to differences in indsutry products and services and the financial leverage of the firms in the industry. Spreads for issuers in the consumer cyclical sector invrease significantly during economic downturns compared to spreads for isseurs in the consumer non-cyclical sector.

산업별로, 시간별로 spread 차이가 발생 - product, service, leverage 차이

## LOS 46.h: Explain how the phase of the business cycle affects short-term and long-term earnings growth expectations.

Cyclical industries tend to be relatively more sensitive to the phase of the business cycle. Companies in these industries have revenues and earnings that rise and fall with the rate of economic growth. Defensive or non-cyclical industries tend to be relatively immune to fluctuations in economic activity; their earnings tend to be relatively stable throughout the business cycle.

1.   cyclical industry -> business cycle에 더 민감, economic growth rate이 중요
2.   defensive -> 상대적으로 덜 영향

## LOS 46.i: Explain the relationship between the consumption-hedging properties of equity and the equity risk premium.

The discount rate used to value equity secutiries includes an additional risk premium, the equity risk premium because equity is more risky than debt.
$$
\\\operatorname{Discount rate for equity} = R + \pi + \theta + \gamma + \kappa
\\\kappa = \text{additional risk premium relative to risky debt for an investment in equities}
\\\lambda = \text{equity risk premium} = \gamma + \kappa
$$
Assets that provide a higher payoff during economic downturns are more highly valued because of the consumption hedging property of the asset. Equity prices are generally cyclical, with higher values during economic expansions when the marginal utility of consumption is lower. Equity investments, therefore, are not the most effective hedge against bad consumption outcomes.

Discount rate = R + inflation + risk premium + y + k

### Consumption hedging property of asset

-   경기침체 시 더 payoff 하는 자산이 good
-   이런 자산은 risk premium이 감소
-   경기확장 시 equity는 가격증가 - cyclical -> 주식투자는 경기침체 시 좋은 hedge 수단이 아님

## LOS 46.j: Describe cyclical effects on valuation multiples.

Price multiples such as P/E and P/B are often used in determining the relative values of companies, of sectors, or of the overall market from a historical perspective. However, it is inappropriate to judge the multiple in a historical context only.

Price multiples are positively correlated with expected earnings growth rates and negatively correlated to required returns.

Shiller's CAPE (real cyclically adjusted P/E) ratio reduces the volatility of unadjusted P/E ratios by using real prices in the numerator and a 10-year moving average of real earnings in the denominator.

Price multiple (P/E, P/B)

-   회사별 sector별 역사적 관점으로 판단 x
-   earning growth %와 price multiple은 상관계수가 +
-   required return과 price multiple은 상관계수가

## LOS 46.k: Describe the implications of the business cycle for a given style strategy (value, growth, small capitalization, large capitalization).

Growth stocks are characterized by high P/Es and by low dividend yields and tend to be in immature markets with high growth prospects. Value stocks tend to have low P/Es, have high dividend yields, and are generally found in established and mature markets. A value strategy performs well during and immediately following recessionary conditions, while growth strategy performs well during economic expansions.

-   Growth = High P/E, Low dividend, 경기확장 시 good
-   Value = low P/E, high dividend, stable earning, 경기침체 시 good

## LOS 46.l: Describe how economic analysis is used in sector rotation strategies.

Ex post risk premiums on equity sectors can be computed as the difference between the average return on a sector and the short-term risk free rate. Getting the timing right is of course very difficult. The point, however, is that understanding and forecasting the relationship between the equity market performance of different sectors and the business cycle would help analysts enhance their sector rotation strategies.

Rotation = cyclical vs. non-cyclical

분석 필요 - correlation, risk premium 등

## LOS 46.m: Describe the economic factors affecting investment in commercial real estate.

Commercial real estate investments have

-   Bond-like characteristics. The steady rental income stream is similar to cash flows from a portfolio of bonds. The credit quality of tenants affects the value of commercial real estate.
-   Equity-like characteristics. The value of commercial real estate is influenced by many factors, including the state of the economy, the demand for rental properties, and property location. Uncertainty about the value of the property at the end of the lease term gives commercial properties an equity-like character.
-   Illiquidity.

### Valuation

$$
\\\operatorname{Discount rate for commercial real estate} = R + \pi + \theta + \gamma + \kappa + \phi
\\\kappa = \text{risk premium for uncertainty about termainal value of property (similar to the equity risk premium)}
\\\phi = \text{risk premium for illiquidity}
$$

성격

-   bond-like - 안정적 임대수입, 임차인에 따라 신용도 영향
-   equity-like - value가 경기에 영향 받음, 임대기간 말에 불확실성 존재

valuation = R + inflation + risk premium + r + k + Rp(비유동성 프리미엄)

상업용 부동산은 가치가 cyclical -> 다른자산과 상관계수 +

## LOS 47.a: Describe how value added by active management is measured.

The information ratio is used to evaluate active managers and can be used to make portfolio allocation decisions for an investor.

Active management seeks to add value by outperforming a passively managed benchmark portfolio.

### Active return

Active return($R_{A}$) is the value added by active management. Active return can be measured ex-ante or ex-post.

Active weights in a portfolio determine the amount of value added. Active weights must sum to zero.

Expected returns on the active and benchmark portfolios can be computed as the weighted average of securities returns:
$$
\\E(R_{P}) = \sum{w_{Pj}E(R_{Pj})}\, and\, E(R_{B}) = \sum{w_{Bj}E(R_{Bj})}
\\E(R_{A}) = \sum{w_{Pj}E(R_{Pj})} - \sum{w_{Bj}E(R_{Bj})}
$$
Active return can be decomposed into two parts:

1.   Asset allocation return
2.   Security selection return

사전적, 사후적으로 측정 가능

## LOS 47.b: Calculate and interpret the information ratio (ex post and ex ante) and contrast it to the Sharpe ratio.

The Sharpe ratio (SR) is calculated as excess return per unit of risk (standard deviation):
$$
\\SR = \frac{R_{P} - R_{F}}{\sigma_{P}}
$$
An important attribute of the Sharpe ratio is that it is unaffected by the addition of cash or leverage in the portfolio.

The information ratio (IR) is the ratio of the active return to the standard deviation of active returns, which is known as active risk:
$$
\\IR = \frac{R_{P} - R_{B}}{\sigma_{(R_{P} - R_{B})}} = \frac{R_{A}}{\sigma_{A}} = \frac{\operatorname{active return}}{\operatorname{active risk}}
$$

### Some important points

-   The information ratio that we are considering is usually the ex-ante information ratio. The ex-ante information ratio is generally positive, while ex-post information ratios will often turn out to be negative.
-   A closet index fund is a fund that is purposed to be actively managed but in reality closely tracks the underlying benchmark index. These funds will have a Sharpe ratio similar to that of the benchmark index, a very low information ratio, and little active risk. After fees, the information ratio of a closet index fund is often negative.
-   A fund with zero systematic risk that uses the risk-free rate as its benchmark would have an information ratio that is equal to its Sharpe ratio.
-   Unlike the Sharpe ratio, the information ratio will change with the addition of cash or the use of leverage. Adding cash to a portfolio is likely to lower active return.
-   The information ratio of an unconstrained portfolio is unaffected by the aggressiveness of the active weights. If the active weights of a portfolio are tripled, the active return and the active risk both triple, leaving the information ratio unchanged.
-   The resulting blended portfolio will have the same information ratio as the original actively managed portfolio, leaving the information ratio unchanged.
-   Investors can select an appropriate amount of active risk by investing a portion of their assets in the active portfolio and the remaining portion in the benchmark.

For an unconstrained active portfolio, the optimal amount of active risk is the level of active risk that maximizes the portfolio's Sharpe ratio. This optimal amount of active risk can be calculated as:
$$
\\\sigma_{A}^{*} = \frac{IR}{SR_{B}}\sigma_{B}
\\SR_{P} = \sqrt{SR_{B}^{2} + IR^{2}}
$$
![image-20211008062653567](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211008062653567.png)

![image-20211008062659880](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211008062659880.png)

## LOS 47.c: State and interpret the fundamental law of active portfolio management including its component terms-transfer coefficient, information coefficient, breadth, and active risk (aggressiveness).

-   The information coefficient (IC) is a measure of a manager's skill. IC is the ex-ante, risk-weighted correlation between active returns and forecasted active returns.
-   The transfer coefficient (TC) can be thought of as the correlation between actual active weights and optimal active weights. For an constrained active portfolio, the active weights will be equal to the optimal weight and TC = 1.
-   Breadth (BR) is the number of independent active bets taken per year.

$$
\\IR = TC * IC * \sqrt{BR}
\\E(R_{A}) = TC * IC * \sqrt{BR} * \sigma_{A}
$$

IR의 3가지 구성항목

-   Information coefficient - manager skill
-   Transfer coefficient - 자유도 정도
-   breadth - number of independent active part

Grinold rule - modified active return 개념

IR을 늘리려면? - IC를 증가시키거나, BR을 늘리거나

## LOS 47.d: Explain how the information ratio may be useful in investment manager selection and choosing the level of active portfolio risk.

Portfolio theory concludes that investors choose some combination of the risk-free asset and an optimal risky portfolio, with the weights determined by their preferences (risk tolerance). The optimal risky portfolio is the portfolio with the highest Sharpe ratio. The portfolio with the highest information ratio will also be the portfolio with the highest Sharpe ratio, so investors will choose the active manager with the highest Sharpe ratio.
$$
\\E(R_{A}) = IR * \sigma_{A}
$$
결론

-   optimization risk portfolio - highest Sharpe ratio
-   Highest IR portfolio - highest Sharpe ratio portfolio

## LOS 47.e: Compare active management strategies (including market timing and security selection) and evaluate strategy changes in terms of the fundamental law of active management.

Market timing is simply a bet on the direction of the market (or a segment of the market).
$$
\\IC = 2(\operatorname{\%\, of\, correct}) - 1
$$

### Sector rotation

Market timing can also be used to make sector rotation decisions.
$$
\\\sigma_{C} = [\sigma_{X}^{2} - 2\sigma{_X}\sigma_{Y}\rho_{XY} + \sigma_{Y}^2]^{1/2}
$$
시장방향에 베팅

우수한 성과를 보이는 sector에 자산 할당

## LOS 47.f: Describe the practical strengths and limitations of the fundamental law of active management.

The practical limitations of the fundamental law of active management can be summarized as "garbage in, garbage out;" poor input estimates lead to incorrect evaluations. In the case of unconstrained optimization, the two components (inputs) that determine the information ratio are 1) the information coefficient (IC) and 2) the breadth (BR) of the manager's strategy.

The limitations are generally derived from inaccurate estimates of the two inputs:

-   Ex-ante measurement of skill - Managers tend to overestimate their ability to outperform the market and, hence, overestimate their IC.
-   Independence - If two or more decisions rely on same (or similar) information, then they are not independent.

$$
\\BR = \frac{N}{1 + (N - 1)r}
\\N = \text{number of decisions}
\\r = \text{correlation between the decisions}
$$

Limitation - ex ante manager skill -  고평가

independence - 진짜 결정이 다 독립적?

그래도 성과평과 input이 적으니 편함

## LOS 48.a: Explain the components of execution costs, including explicit and implicit costs.

Evaluation of trade execution should not only consider explicit costs such as brokerage fees but also implicit costs.

### Trading costs

Explicit trading costs include brokerage, taxes, and fees.

Implicit costs are harder to measure, and include the bid-ask spread, market or price impact costs, opportunity costs, and delay costs (or slippage).

-   The bid-ask spread is the highest potential cost for a small trade.
-   Market impact (or price impact) is the impact of demanding illiquidity in the market.
-   Delay cost (or slippage) is the cost of an adverse price movement during the lag in executing a large trade.
-   Opportunity cost arises from unfilled orders or failed trading opportunities.

Note that there is a tradeoff between the market impact cost on one hand and the delay plus opportunity cost on the other.

1.   Explicit cost - brokerage, taxes, fee
2.   Implicit cost - Bid-ask spread, market impact, delay cost, opportunity cost

tradeoff 존재 - market impact vs delay + opportunity cost

## LOS 48.b: Calculate and interpret effective spreads and VWAP transaction cost estimates.

Larger orders have a price impact as they move down the order book (and, therefore, execute at worse prices). This price impact depends on the size of the order and the relative liquidity in the market.

Dealer는 거래중개인

bid = 삽니다 / ask = 팝니다 -> 둘 사이 차이는 inside spread, 중간은 midquote

large order는 price impact 존재 (해당 단가에 물량이 별로 없다면) -> 대안으로 standing limit order (지정가 주문), 그러나 체결이 안 될 위험있음

### Types of benchmarks

The implicit costs of a trade are measured relative to a benchmark. Several benchmarks can be used to evaluate trades, including the effective spread, VWAP, and implementation shortfall.

#### Effective spread

The effective spread transactions cost uses the midquote price as the benchmark price.
$$
\\\operatorname{per-share\, effective\, spread\, transaction\, cost} = \operatorname{side} + (\operatorname{transaction price} - \operatorname{midquote price})
\\\operatorname{side} = \text{+1 for buy orders and -1 for sell orders}
\\\operatorname{effective spread} = 2 * \operatorname{per-share\, effective\, spread\, transaction\, cost}
$$
If the trade occurs at a better price, there will be a price improvement.

Since the effective spread is less than the quoted spread, there was not a price improvement on that trade.

Limitations of effective spread

-   When a larger order is split into smaller orders, the effective spread is a poor indicator of trade performance.
-   Effective spread also does not account for slippage or delay costs when part of the order does not get filled at desired prices.
-   Effective spread does not capture the opportunity cost of a trade.

Spread는 낮을수록 거래를 잘한 것

단점 - 거래량을 무시 -> delay cost, opportunity cost 반영 못함 (거래가 이루어지지 않았을 경우)

#### Volume-weighted average price (VWAP)

VWAP is easy to interpret-it evaluates the price at which an order was executed relative to other trades occurring during the same time period.

To evaluate a trade, the VWAP of the trade is compared to the benchmark VWAP.
$$
\\\operatorname{VWAP transaction cost} = \operatorname{trade size} * \operatorname{side} * (\operatorname{trade VWAP} - \operatorname{benchmark VWAP})
$$
Limitations of VWAP transaction cost

-   VWAP is not useful if the trade being evaluated is a significant part of the trading volume.
-   VWAP does not capture the price impact cost.

하루에 거래한 내역들을 가중평균(거래량 기준)한 가격

BM VWAP과 비교

단점 - 거래량이 영향 -> 거래량이 너무 많으면 BM과 별 차이 없어짐, price impact cost 반영 못함 (단 1개의 거래로 가격이 상승했을 경우)

VWAP의 탄생 -> 장 마감 직전까지 기다렸다가 거래를 하려는 manager들이 생김 -> implementation shortfall 탄생

## LOS 48.c: Describe the implementation shortfall approach to transaction cost measurement.

### Implementation shortfall

Implementation shortfall is a conceptual approach that measure transactions costs as the difference between the value of the actual portfolio and the value of hypothetical paper portfolio.

It measures the total cost of trading by capturing all three implicit costs (i.e., price impact, slippage, and opportunity costs).

paper portfolio와 actual portfolio를 비교

paper portfolio는 가상의 portfolio로 trade가 모두 원래 계왹한 가격에 이루어졌다고 가정 -> actual과의 비교로 price impact, slippage, opportunity costs 모두 잡아냄

## LOS 48.d: Describe factors driving the development of electronic trading systems.

The use of information technology in the development of electronic markets has resulted in lower trading costs and improved execution efficiency.

Factors driving development of electronic trading systems are

-   Cost
-   Accuracy
-   Audit trails
-   Fraud prevention
-   Continuous market

Bond market trades remain largely over the counter.

기술발달 -> 수요공급자들을 보다 빠르게 연결 -> trading cost 감소, 거래효율성 증가

장점 - costs, accuracy, audit trail, fraud prevention, continuous market

주식시장 대부분 electronic trading, 그러나 아직 채권시장은 dealer에게 많이 의존 (OTC)

## LOS 48.e: Describe market fragmentation.

Market fragmentation occurs when a security trades in multiple markets.

Automated trading strategies for large orders seek out liquidity across all markets to minimize the price impact of their trades.

특정주식이 여러시장에서 거래될 때 -> market fragmentation 발생 -> 각 시장의 liquidity 차이로 cost 발생 가능

대안 - 자동화 기술 -> liquidity aggregation - 모든 시장을 다 뒤짐 / smart order - 제일 효율적인 시장 고름

## LOS 48.f: Distinguish among types of electronic traders.

### Electronic news traders

These analyze high-speed news feeds and submit market orders (as opposed to limit orders) based on the analysis.

뉴스를 빠르게 분석하여 시장 거래, AI 사용하기도 함

### Electronic dealers

These post bid and offer prices to profit from the spread. Dealer profit depends on the frequency with which they trade, Electronic dealers maintain a low inventory of actively traded securities and quickly adjust their positions based on market information.

Bid-ask spread로 이익 추구, low inventory (빠르게 position이 adjusted되어서)

### Electronic arbitrageurs

These trade in multiple markets seeking to exploit price discrepancies.

price discrepancies 찾아다님

### Electronic front runners

These use artificial intelligence to sniff out large trades (or many small trades) on the same side and then use low latency to trade ahead of them. Front runners search for patterns in order submissions or relationships between orders and events.

빠르게 행동하는 trader, 대량거래 발생 전에 해당주식 매수하여 매도 (pattern과 event를 분석)

### Electronic quote matchers

Standing limit orders provide valuable information to other traders; they disclose the intend of the trader posting the order to buy or sell the specified quantity.

특정가격에 매수/매도 주문 -> 그 자체만으로도 다른 trader들에게 의미있는 정보

### Buy-side traders

These execute trades on behalf of their portfolio managers.

portfolio manager의 주문을 받아 대신 거래하는 trader

## LOS 48.h: Describe comparative advantages of low-latency traders.

In addition to lower trading costs, electronic trading system allow low-latency traders a competitive advantage by jumping the order queue. In other words, electronic traders have to be faster than their competitors to capitalize on market opportunities.

Low-latency traders focus on minimizing the latency involved in three phases of a trade:

1.   The time gap between the publication of actionable news and the receipt of that news by the trader.
2.   The time gap between the receipt of actionable news and deciding on an appropriate action.
3.   The time gap between order determination and communicating that order to the exchange.

-   Communication speed
-   Computation speed

electronic trading -> low latency, 대응속도가 빨라짐 -> 과거보다 빠르게 시장의 개회를 capture 가능

1: 시장에서 정보의 발생 -> 2: trader가 정보를 취득 -> 3: trader가 의사결정 후 명령 -> 4: 거래 수행

2, 4: communication speed

3: computation speed

## LOS 48.g: Describe characteristics and uses of electronic trading systems.

Advanced order types are limit orders with a dynamic limit price that varies with a benchmark.

Trading tactics are plans calling for the submission of multiple orders.

Algorithms (or algos) are programmed execution strategies using multiple orders, sequencing of orders, and trading tactics to achieve specific goals.

### Impact of electronic trading

1.   Hidden orders
2.   Leapfrog - This is the practice of beating the best bid or ask price. A leapfrogging limit order therefore narrows the inside spread.
3.   Flickering quotes - These are exposed limit orders that are submitted and canceled almost immediately.
4.   Electronic arbitrage
     1.   Take liquidity on both sides - This is an arbitrage trade to buy and sell the same security in different markets to take advantage of mispricing across markets.
     2.   Offer liquidity on one side
     3.   Offer liquidity on both sides - This strategy is fraught with risks; after one leg of the order is filled, if the other leg does not fill, the trader is exposed to risk of adverse price movement.
5.   Machine learning - Also known as data mining, machine learning involves using statistical modeling techniques that allow the model to evolve based on new data.

advanced order type - limit order with a dynamic limit price

![image-20211008074458164](/Kevin_Min/images/2021-10-05-CFA-Level-2-Portfolio-Management/image-20211008074458164.png)

algorithms - 미리 설정&프로그램 된 전략으로 trading

Electronic trading의 영향

1.   hidden orders - 기존 거래방식(bid-ask)을 따르지 않고, 거래정보(단가, 규모)를 공개하지 않은 상태로 거래
2.   leapfrog - ask 관련 dealer들의 경쟁 심화 -> bid-ask spread가 좁혀짐
3.   flickering quotes - 주문 후 바로 취소, 상대방이 해당 주문 가격으로 먼저 제안하기를 바라는 전략 (우리 물량은 공개하기 싫을 때)
4.   arbitrage
     1.   take liquidity on both sides - 다른 시장에서 다른 가격으로 판매되는 security들을 동시에 buy&sell (market order)
     2.   offer liquidity on one side - 특정주식을 싼 시장에서 사서 비싼시장에 팔기 (limit order)
     3.   offer liquidity on both sides - 특정주식을 best 가격보다 비싸게 사서 다른 시장에 팔기 (limit order) -> 위험노출
5.   machine learning - data mining, 통계, 새로운 data로 알고리즘 개발 -> 극단 case에는 안 들어 맞을수도

## LOS 48.i: Describe the risks associated with electronic trading and how regulators mitigate them.

-   High-frequency traders (HFT) arms race - This arms race offsets some of the lower cost benefits of electronic trading.
-   Systemic risk
    -   Runaway algorithms - These produce a series of unintended orders. The flash crash of May 2010 was caused by a trading algorithm.
    -   Fat finger errors - These are input errors.
    -   Overcharging orders - These demand liquidity significantly higher than what is available in the market.
    -   Malevolent orders - These are created to specifically manipulate the market. Examples includes aggrieved employees programming rogue trades and traders seeking to conduct denial-of-service attacks on their competitors with excessive submission of quotes.

high-frequency trader (HFT) arms race - 최첨단 시설 구축으로 인한 비용 (cost 증가)

systematic risk - 기술의 발달로 인해 피해자들이 발생할 수 있음

-   runaway algorithms, fat finger errors, overcharge orders, malevolent orders

## LOS 48.j: Describe abusive trading practices that real-time surveillance of markets may detect.

-   Front running -This is low-latency trading ahead of known large trades.
-   Market manipulation - This includes activities that produce false market data, including price and volume data.
    -   Trading for market impact - These are trades designed to change the price.
    -   Rumormongering - This involves dissemination of fake information to affect the target trader's value assessments.
    -   Wash trading - This is trading between commonly controlled accounts to create an impression of false liquidity.
    -   Spoofing or layering - These are fake limit orders posted to create fake optimism or pessimism about the security.
    -   Bluffing - This involves preying on momentum traders.
    -   Gunning the market - This focuses other traders into bad trades.
    -   Squeezing and cornering

front running - low-latency trading head of known large trade

market manipulation - 거짓된 data로 시장 조작

-   trading for market impact (시장가격 영향주기)
-   rumormongering (루머)
-   wash trading (자전거래)
-   spoofing & layering (optimism 또는 pessimism으로 시장가보다 다른 가격 제시, 시장 흔들기)
-   bluffing - 모멘텀 투자자들
-   gunning the market - stop-loss 주문한 투자자들 노리기, 대량 short하여 나오는 물량 사기
-   squeezing & cornering - 상대방으로 default 위험에 처하게 해서 이익 추구
