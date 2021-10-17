---
toc: true
layout: post
description: CFA Level 2 Corporate Finance summary
categories: [markdown]
title: CFA Level 2 Corporate Finance
---
# CFA Level 2 Corporate Finance

## Corporate Finance Overview

![image-20211017200234167](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200234167.png)

![image-20211017200326244](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200326244.png)

![image-20211017201059307](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017201059307.png)

## LOS 19.a: Calculate the yearly cash flows of expansion and replacement capital projects and evaluate how the choice of depreciation method affects those cash flows.

![image-20211017201115435](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017201115435.png)

![image-20211017201126107](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017201126107.png)

![image-20211017201135147](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017201135147.png)

![image-20211017201142808](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017201142808.png)

The relevant cash flows for evaluating a capital project are the incremental after-tax cash flows. How various real options give managers flexibility with capital budgeting projects. Even if you are unsure how to handle the calculation of NPV involving real options, remember that the existence of options will always increase NPV. Finally, familiarize yourself with alternative concepts of calculating income, including economic income, economic profit, residual income, and claims analysis, and pay attention to the proper discount rate under each method.

### Cash flow estimation

#### Basics of capital budgeting

The capital budgeting process is the process of identifying and evaluating capital projects; that is, projects where the cash flow to the firm will be received over a period longer than a year. Any corporate decisions with an impact on future earnings can be examined using the framework. Decisions about whether to buy a new machine, expand business in another geographic area, move the corporate headquarters to Cleveland, or replace a delivery truck, to name a few, can be examined using a capital budgeting analysis.

#### Categories of capital budgeting projects

-   Replacement projects to maintain the business
-   Replacement projects for cost reduction
-   Expansion projects
-   New product or market
-   Mandatory projects
-   Other projects

#### Principles of capital budgeting

1.   Decisions are based on cash flows, not accounting income.

     The relevant cash flows to consider as part of the capital budgeting process are incremental cash flows.

     Sunk costs are costs that cannot be avoided, even if the project is not undertaken. (과거 cost는 고려하지 않음) An example of a sunk cost is a consulting fee paid to a marketing research firm to estimate demand for a new product prior to a decision on the project.

     Externalities - cannibalization

     -   pre-emptive cannibalization - 시장 선점 목적, 수익률은 떨어지지만 NPV 극대화

2.   Cash flows are based on opportunity costs.

3.   The timing of cash flows is important.

     Capital budgeting decisions account for the time value of money, which means that cash flows received earlier are worth more than cash flows to be received later.

4.   Cash flows are analyzed on an after-tax basis.

5.   Financing costs are reflected in the project's required rate of return.

     The required rate of return is a function of its risks.

### Modified accelerated cost recovery system (MACRS)

case by case로 적용되서 보통 table을 제시하는데, 정 안주면 Double-declining method로 depreciation 계싼하면 됨.

In the United States, modified accelerated cost recovery system (MACRS) for tax purposes.

![image-20211017195221848](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017195221848.png)

The depreciable basis is equal to the purchase price plus any shipping or handling and installation costs. The basis is not adjusted for salvage value regardless of whether the accelerated or straight-line method is used.

Salvage value 고려 않고 0까지 deprecation in tax.

### Incremental cash flows

-   Initial investment outlay is the up-front costs associated with the project. Components are price, which includes shipping and installation (FCInv) and investment in net working capital (NWCInv)

$$
\\\operatorname{outlay} = \operatorname{FCInv} + \operatorname{NWCInv}
\\\operatorname{NWCInv} = \Delta\operatorname{non-cash\, current\, assets} - \Delta\operatorname{non-debt\, current\, liabilities} = \Delta\operatorname{NWC}
$$

-   After-tax operating cash flows (CF)

$$
\\CF = (S - C - D)(1 - T) + D
\\= (S - C)(1 - T) + TD
\\= EBITDA(1 - t) + Dep * t
\\= EBIT(1 - t) + Dep
$$

In general, a higher depreciation expense will result in greater tax savings and higher cash flows. This means that accelerated depreciation methods will create higher after-tax cash flows for the project earlier in the project's life as compared to the straight-line method, resulting in a higher net present value (NPV) for the project.

Interest is not included in operating cash flows for capital budgeting purposes because it is incorporated into the project's cost of capital.

-   Terminal value after-tax non-operating cash flows (TNOCF)

$$
\\TNOCF = Sal_{T} + NWCInv - T(Sal_{T} - B_{T})
\\Sal_{T} = \text{pre-tax cash procedds from sale of fixed capital}
\\B_{T} = \text{book value of the fixed capital sold}
$$

![image-20211017200110833](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200110833.png)

![image-20211017200117903](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200117903.png)

![image-20211017200356823](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200356823.png)

### Replacement project analysis

증분고려

![image-20211017200148649](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200148649.png)

![image-20211017200154973](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200154973.png)

![image-20211017200202853](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200202853.png)

![image-20211017200209278](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200209278.png)

![image-20211017200422080](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200422080.png)

## LOS 19.b: Explain how inflation affects capital budgeting analysis.

Inflation is a complication.

-   Analyzing nominal or real cash flows. - Nominal cash flows should be discounted at a nominal discount rate, while real cash flows should be discounted at a real discount rate.
    -   rate adjusted for inflation -> real rate
-   Changes in inflation affect project profitability. - If inflation is higher than expected, future project cash flows are worth less, and the value of the project will be lower than expected. The opposite is also true, however. If inflation turns out to be lower than originally expected, future cash flows from the project will be worth more, effectively increasing the project's value.
-   Inflation reduces the tax savings from deprecation.
-   Inflation decreases the value of payments to bondholders.
-   Inflation may affect revenues and costs differently.

## LOS 19.c: Evaluate capital projects and determine the optimal capital project in situations of 1) mutually exclusive projects with unequal lives, using either the least common multiple of lives approach or the equivalent annual annuity approach, and 2) capital rationoing.

### Mutually exclusive projects with different lives

When two projects are mutually exclusive, the firm may choose one project or the other, but not both. It mutually exclusive projects have different lives, and the projects are expected to be replaced indefinitely as they wear out, an adjustment needs to be made in the decision-making process.

1.   Least common multiple of lives approach -  최소공배수법
2.   Equivalent annual annuity (EAA) approach

![image-20211017200951691](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200951691.png)

![image-20211017200957730](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017200957730.png)

![image-20211017201011848](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017201011848.png)

![image-20211017201023378](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017201023378.png)

![image-20211017201029806](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017201029806.png)

![image-20211017202636161](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017202636161.png)

![image-20211017202642823](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017202642823.png)

### Capital rationing

Capital rationing is the allocation of a fixed amount of capital among the set of available projects that will maximize shareholder wealth. Greatest total NPV.

Note that capital rationing is not the optimal decision from the firm's perspective. Therefore, capital rationing violates market efficiency because society's resources are not allocated to their best use (i.e., to generate the highest return).

Hard capital rationing occurs when the funds allocated to managers under the capital budget cannot be increased. Soft capital rationing occurs when managers are allowed to increase their allocated capital budget if they can justify to senior management that the additional funds will create shareholder value.

![image-20211017202000892](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017202000892.png)

![image-20211017202006586](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017202006586.png)

## LOS 19.d: Explain how sensitivity analysis, scenario analysis, and Monte Carlo simulation can be used to assess the stand-alone risk of a capital project.

Sensitivity analysis involves changing an input (independent) variable to see how sensitive the dependent variable is to the input variable. For example, by varying sales, we could determine how sensitive a project's NPV is to changes in sales, assuming that all other factors are held constant. The key to sensitivity analysis is to only change one variable at a time.

![image-20211017202315045](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017202315045.png)

Scenario analysis is a risk analysis technique that considers both the sensitivity of some key output variable to changes in a key input variable and the likely probability distribution of these variables. The key difference between scenario analysis and sensitivity analysis is that scenario analysis allows for changes in multiple input variables all at once.

![image-20211017202309221](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017202309221.png)

Simulation analysis (or Monte Carlo simulation) results in a probability distribution of project NPV outcomes, rather than a limited number of outcomes as with sensitivity or scenario analysis.

![image-20211017202358612](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017202358612.png)

## LOS 19.e: Explain and calculate the discount rate, based on market risk methods, to use in valuing a capital project.

$$
\\R_{project} = R_{F} + \beta_{project}[E(R_{MKT}) - R_{F}]
$$

Using a project's beta to determine discount rates is important when the risk of a project is different from the risk of the overall company. Simply using the company's weighted average cost of capital (WACC) will overstate the required return for a conservative (low beta) project and will understate the required return for an aggressive (high beta) project.

## LOS 19.f: Describe types of real options and evaluate a capital project using real options.

Real options allow managers to make future decisions that change the value of capital budgeting decisions made today.

-   Timing options
-   Abandonment options are similar to put options. They allow management to abandon a project if the present value of the incremental cash flows from exiting a project exceeds the present value of the incremental cash flows from continuing a project.
-   Expansion options are similar to call options.
-   Flexibility options
    -   price-setting
    -   production-flexibility
-   Fundamental options are projects that are options themselves because the payoffs depend on the price of an underlying asset. For example, the payoff for a copper mine is dependent on the market price for copper.

Different approaches for evaluating the profitability of an investment with real options.

-   Determine the NPV of the project without the option.
-   Calculate the project NPV without the option and add the estimated value of the real option
-   Use decision trees
-   Use option pricing models

![image-20211017203306791](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017203306791.png)

![image-20211017203313306](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017203313306.png)

![image-20211017203319965](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017203319965.png)

![image-20211017202651779](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017202651779.png)

## LOS 19.g: Describe common capital budgeting pitfalls.

Common mistakes

-   Failing to incorporate economic responses into the analysis
-   Misusing standardized templates
-   Pet projects of senior management - 경영자 선호 project
-   Basing investment decision on EPS or ROE
-   Using the IRR criterion for project decisions
-   Poor cash flow estimation
-   Misestimation of overhead costs
-   Using the incorrect discount rate
-   Politics involved with spending the entire capital budget - Many managers try to spend their entire capital budget each year and ask for an increase for the following year.
-   Failure to generate alternative investment ideas
-   Improper handling of sunk and opportunity costs

## LOS 19.h: Calculate and interpret accounting income and economic income in the context of capital budgeting.

Economic income
$$
\\\operatorname{economic income} = \operatorname{cash flow} + (\operatorname{ending market value} - \operatorname{beginning market value}) = \operatorname{cash flow} - \operatorname{economic depreciation}
$$
A project's accounting income is the reported net income on a company's financial statements that results from an investment in a project. Accounting income will differ from economic income because:

-   Accounting depreciation is based on the original cost (not market value) of the investment.
-   Financing costs are considered as a separate line item and subtracted out to arrive at net income. In the basic capital budgeting model, financing costs are reflected in the WACC.

![image-20211017203855837](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017203855837.png)

![image-20211017203901374](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017203901374.png)

![image-20211017203907124](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017203907124.png)

The accounting income differs from the economic income for two reasons.

1.   Accounting depreciation is based on the original cost of the investment, while economic depreciation (beginning - ending value) is based on the market value of the asset. The economic depreciation for the project is much larger than the accounting depreciation, resulting in an economic income amount that is much smaller than accounting income.
2.   Interest expense is deducted from the accounting income figure. Interest expense is ignored when computing economic income because it is reflected in the WACC.

## LOS 19.i: Distinguish among the economic profit, residual income, and claims valuation models for capital budgeting and evaluate a capital project using each.

Economic profit is a measure of profit in excess of the dollar cost of capital invested in a project.
$$
\\EP = NOPAT - \$WACC
\\NOPAT = \text{net operating profit after tax} = EBIT(1 - t)
\\\$WACC = \text{dollar cost of capital} = WACC * capital
\\Capital = \text{dollar amount of investment}
$$
![image-20211017204716763](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017204716763.png)
$$
\\NPV = MVA = \sum_{t = 1}^{\infty}{\frac{EP_{t}}{(1 + WACC)^{t}}}
\\MVA = \text{market value added}
$$
Residual income focuses on returns on equity and is determined by subtracting an equity charge from the accounting net income.
$$
\\\operatorname{residual income} = \operatorname{net income} - \operatorname{equity charge}
\\RI_{t} = NI_{t} - r_{e}B_{t - 1}
\\NPV = \sum_{t = 1}^{\infty}{\frac{RI_{t}}{(1 + r_{e})^{t}}}
$$
The residual income approach focuses only on returns on equityholders; therefore, the appropriate discount rate is the required return on equity.

![image-20211017205118120](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205118120.png)

![image-20211017205123097](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205123097.png)

The claims valuation approach (청구권 방식, FCFF, FCFE 활용) divides operating cash flows based on the claims of debt and equityholders that provide capital to the company. These debt and equity cash flows are valued separately and then added together to determine the value of the company.

The claims valuation method calculate the value of the company not the project. This is different from the economic profit and residual income approaches, which calculate both project and company value.

The claims valuation approach is based on the balance sheet concept that assets equal liabilities plus equity.

-   The cash flows to debtholders consist of interest and principal payments and are discounted at the cost of debt.
-   The cash flows to equityholders are dividends and share repurchases and are discounted at the cost of equity.

The sum of the present value of each stream of cash flows will equal the value of the company.

![image-20211017205412535](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205412535.png)

![image-20211017205421790](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205421790.png)

![image-20211017205532597](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205532597.png)

![image-20211017205538033](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205538033.png)

![image-20211017205544205](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205544205.png)

![image-20211017205550042](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205550042.png)

![image-20211017205556196](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205556196.png)

![image-20211017205601907](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205601907.png)

![image-20211017205607235](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205607235.png)

![image-20211017215634145](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215634145.png)

![image-20211017215641187](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215641187.png)

![image-20211017215647237](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215647237.png)

![image-20211017215654934](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215654934.png)

## LOS 20.a: Explain the Modigliani-Miller propositions regarding capital structure, including the effects of leverage, taxes, financial distress, agency costs, and asymmetric information on a company's cost of equity, cost of capital, and optimal capital structure.

![image-20211017205619151](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017205619151.png)

### Overview of the capital structure theories

Progression is from MM 1958 (no taxes, no costs of financial distress) to MM 1963 (with taxes, no costs of financial distress) to the static trade-off theory (with taxes and with costs of financial distress).

In moving to MM 1963, we are able to see how introducing taxes affects the cost of capital and firm value. Remember, the goal of managers in a capital structure decision is to minimize the weighted average cost of capital (and thereby maximize the value of the company).

### MM Proposition I (no taxes): The capital structure irrelevance proposition

In 1958, Professors Franco Modigliani and Merton Miller (MM) published their seminal work on capital structure theory. Under a very restrictive set of assumptions, MM proved that the value of a firm is unaffected by its capital structure. MM's results suggest that in a perfect world, it does not matter how a firm finances its operations.

Assumptions

-   Capital markets are perfectly competitive - There are no transaction costs, taxes, or bankruptcy costs.
-   Investors have homogeneous expectations
-   Riskless borrowing and lending - Investors can borrow/lend at the risk-free rate.
-   No agency costs - No conflict of interest between managers and shareholders.
-   Investment decisions are unaffected by financing decisions - Operating income is independent of how assets are financed.

In the MM no-tax world, the value of a company is not affected by its capital structure.

![image-20211017213434459](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017213434459.png)

Consider why the pie analogy holds true. The operating earnings (EBIT) of a firm are available to all providers of capital. In a company with no debt, all of the operating earnings are available to equityholders, and the value of the company is the discounted present value of these earnings.
$$
\\V_{L} = V_{U}
\\V_{L} = \text{value of levered firm}
\\V_{U} = \text{value of unlevered firm}
$$
Given our assumptions, an investor can have homemade leverage.

### MM proposition II (no taxes): Cost of equity and leverage proposition

MM's second proposition with no taxes states that the cost of equity increases linearly as a company increases its proportion of debt financing. Therefore, the benefits of using a larger proposition of debt as a cheaper source of financing are offset by the rise in the cost of equity, resulting in no change in the firm's weighted average cost of capital (WACC).
$$
\\r_{e} = r_{0} + \frac{D}{E}(r_{0} - r_{d})
$$
As leverage increases, the cost of equity increases, but WACC and the cost of debt are unchanged.

![image-20211017213748033](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017213748033.png)

MM's second proposition supports their first proposition. Because the benefits of lower cost debt are offset by the increased cost of equity, the relative amount of debt versus equity in the firm's capital structure does not affect the overall value of the firm.

### MM Proposition I (with taxes): Value is maximized at 100% debt

Tax shield provided by debt. Under the tax code of most countries, interest payments are a pretax expense and are therefore tax deductible, while dividends are paid on an after-tax basis. The differential tax treatment encourages firms to use debt financing because debt provides a tax shield that adds to the value of the company.
$$
\\V_{L} = V_{U} + t * d
$$
If we maintain MM's other assumptions, the value of the company increases with increasing levels of debt, and the optimal capital structure is 100% debt.

### MM Proposition II (with taxes): WACC is minimized at 100% debt

$$
\\r_{E} = r_{0} + \frac{D}{E}(r_{0} - r_{D})(1 - T_{C})
$$

![image-20211017214135286](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017214135286.png)

### Costs and their potential effect on the capital structure

Costs of financial distress - static-trade-off theory (1973)

-   Costs of financial distress and bankruptcy can be direct or indirect. Direct costs of financial distress include the cash expenses associated with the bankruptcy, such as legal fees and administrative fees. Indirect costs include foregone investment opportunities and the costs that result from losing the trust of customers, creditors, suppliers, and employees.
-   Probability of financial distress is related to the firm's use of operating and financial leverage.

Agency costs of equity refer to the costs associated with the conflicts of interest between managers and owners. Managers who do not have a stake in the company do not bear the costs associated with excessive compensation or taking on too much (or too little) risk.

Net agency cost of equity

-   Monitoring costs
-   Bonding costs
-   Residual losses

According to agency theory, the use of debt forces managers to be disciplined with regard to how they spend cash because they have less free cash to use for their own benefit.

Cost of asymmetric information refer to costs resulting from the fact that managers typically have more information about a company's prospects and future performance that owners or creditors. Firms with complex products or little transparency in financial statements tend to have higher costs of asymmetric information, which results in higher required returns on debt and equity capital.

Because shareholders and creditors are aware that the asymmetric information problems exist, these investors will look for management behavior that 'signals' what knowledge management may have. Specifically, management's choice of debt or equity financing may provide a signal regarding management's opinion of the firm's future prospects.

-   Taking on the commitment to make fixed interest payments through debt financing sends a signal that management has confidence in the firm's ability to make these payment in the future.
-   Issuing equity is typically viewed as a negative signal that managers believe a firm's stock is overvalued.

Pecking order theory, based on asymmetric information, is related to the signals management sends to investors through its financing choices. Financing choices under pecking order theory follow a hierarchy based on visibility to investors with internally generated capital being the most preferred, debt being the next best choice, and external equity being the least preferred financing option.

-   Internally generated equity (RE)
-   Debt
-   External equity (newly issued shares)

Therefore, the pecking order theory predicts that the capital structure is a by-product of the individual financing decisions.

### Static trade-off theory

The static trade-off theory seeks to balance the costs of financial distress with the tax shield benefits from using debt. Under the static trade-off theory, there is an optimal capital structure that has an optimal proportion of debt.

If we remove the assumption that there are no costs of financial distress, there comes a point where the additional value added from the debt tax shield is exceeded by the value-reducing costs of financial distress from the additional borrowing. This point represents the optimal capital structure for a firm where the WACC is minimized and the value of the firm is maximized.
$$
\\V_{L} = V_{U} + t * d - PV(\operatorname{costs of financial distress})
$$
![image-20211017215247369](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215247369.png)

![image-20211017215253064](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215253064.png)

![image-20211017215339695](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215339695.png)

![image-20211017215347996](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215347996.png)

![image-20211017215406596](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215406596.png)

![image-20211017215430554](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215430554.png)

![image-20211017215443414](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215443414.png)

![image-20211017215521917](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215521917.png)

![image-20211017215545652](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215545652.png)

![image-20211017215552466](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017215552466.png)

## LOS 20.b: Describe target capital structure and explain why a company's actual capital structure may fluctuate around its target.

Target capital structure

For managers trying to maximize the value of the firm, the target capital structure will be the same as the optimal capital structure.

-   Management may choose to exploit opportunities in a specific-financing source. For example, a temporary rise in the firm's stock price may create a good opportunity to issue additional equity.
-   Market value fluctuations will occur. Changes in stock and bond markets will cause fluctuations in the firm's stock and bond prices.

## LOS 20.c: Describe the role of debt ratings in capital structure policy.

Debt ratings

![image-20211017220434928](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017220434928.png)

## LOS 20.d: Explain factors an analyst should consider in evaluating the effect of capital structure policy on valuation.

-   Changes in the company's capital structure over time.
-   Capital structure of competitors with similar business risk.
-   Company-specific factors (e.g., quality of corporate governance)

## LOS 20.e: Describe international differences in the use of the financial leverage, factors that explain these differences, and implications of these differences for investment analysis.

![image-20211017220611233](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017220611233.png)

## LOS 21.a: Describe the expected effect of regular cash dividends, extra dividends, liquidating dividends, stock dividends, stock splits, and reverse stock splits on shareholders' wealth and a company' financial ratios.

![image-20211018040012018](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018040012018.png)

![image-20211018040552671](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018040552671.png)

![image-20211018040600842](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018040600842.png)

![image-20211017220732343](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017220732343.png)

1.   Regular cash dividends
2.   Extra or special (irregular) dividends
3.   Liquidating dividend
4.   Stock dividend
5.   Stock splits

## LOS 21.b: Compare theories of dividend policy and explain implications of each for share value given a description of a corporate dividend action.

Dividend irrelevance. Merton Miller and Franco Modigliani (MM) maintain that dividend policy is irrelevant, as it has no effect on the price of a firm's stock or its cost of capital. MM's argument of dividend irrelevance is based on their concept of homemade dividends. Assume, for example, that you are a shareholder and you don't like the firm's dividend policy. If the firm's cash dividend is too big, you can just take the excess cash received and use it to buy more of the firm's stock. If the cash dividend you received was too small, you can sell a little bit of your stock in the firm to get the cash flow you want. In either case, the combination of the value of your investment in the firm and your cash in hand will be the same.

Bird-in-hand (dividend preference theory) argument for dividend policy.

Myron Gordon and John Lintner, however, argue that $r_{s}$ decreases as the dividend payout increases. Why? Because investors are less certain of receiving future capital gains from the reinvested earnings than they are of receiving current (and therefore certain) dividend payments.

Tax aversion. In many countries, dividends have historically been taxed at higher rates than capital gains. In the 1970s, US tax rates on dividend income were as high as 70%, while the taxes on capital gains were 35%.

In the real world, tax laws often prevent companies form accumulating excess earnings, making dividend payments necessary. Also note that in 2003, tax laws in the United States changed so that dividends and long-term capital gins are both taxed at the same 15% rate.

Conclusions from the three theories. The results of empirical tests are unclear as to which of these theories best explains the empirical observations of dividend policy.

## LOS 21.c: Describe types of information (signals) that dividend initiations, increases, decreases, and omissions may convey.

Information asymmetry refers to differences in information available to a company's board and management (insiders) as compared to the investors (outsiders).

The information conveyed by dividend initiation is ambiguous. On one hand, a dividend initiation could mean that a company is optimistic about the future and is sharing its wealth with stockholders-a positive signal. On the other hand, initiating a dividend could mean that a company has a lack of profitable reinvestment opportunities-a negative signal.

An unexpected dividend increase can signal to investors that a company's future business prospects are strong and that managers will share the success with shareholders. Studies have found that companies with a long history of dividend increase, such as GE and Exxon Mobil, are dominant in their industries and have high returns on assets and low debt ratios.

Unexpected dividend decreases or omissions are typically negative signals that the business is in trouble and that management does not believe that the current dividend payment can be maintained.

market에 시그널을 줄 수 있다.

## LOS 21.d: Explain how clientele effects and agency costs may affect a company's payout policy.

### Other dividend policy theories

Clientele effect. This refers to the varying dividend preferences of different groups of investors, such as individuals, institutions, and corporations.

-   Tax considerations - High-tax-bracket investors (like some individuals) tend to prefer low dividend payouts, while low-tax-bracket investors (like corporations and pension funds) may prefer high dividend payouts.

When the stock goes ex-dividend:
$$
\\\Delta{P} = \frac{D(1 - T_{D})}{1 - T_{CG}}
$$

-   Requirements of institutional investors. For legal or strategic reasons, some institutional investors will invest only in companies that pay a dividend or have a dividend yield above some target threshold.

### Agency costs

Between shareholders and managers: Agency costs reflect the inefficiencies due to divergence of interests between managers and stockholders. One aspect of agency issue is that managers may have an incentive to overinvest ("empire building"). This may lead to investment in some negative NPV projects, which reduces stockholders wealth. One way to reduce agency cost is to increase the payout of free cash flow as dividends. Generally, it makes sense for growing firms to retain a larger proportion of their earnings.

Between shareholders and bondholders: When there is risky debt outstanding, shareholders can pay themselves a large dividend, leaving the bondholders with a lower asset base as collateral.

![image-20211018004125250](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018004125250.png)

## LOS 21.e: Explain factors that affect dividend policy in practice.

1.   Investment opportunities - If a firm faces many profitable investment opportunities and has to react quickly to capitalize on the opportunities, the dividend payout may be low.
2.   Expected volatility of future earnings - Hence, when earnings are volatile, firms are more cautious in changing dividend payout.
3.   Financial flexibility - Firms with excess cash and a desire to maintain financial flexibility may resort to stock repurchases instead of dividends as a way to pay out excess cash. Since stock repurchase plans are not considered sticky (i.e., there is no implicit expectation by the market of an ongoing repurchase program), they don't entail reduction in financial flexibility going forward.
4.   Tax considerations - Investors are concerned about after-tax returns.
5.   Floatation costs - When a company issues new shares of common stock, a floatation cost of 3% to 7% is taken from the amount of capital raised to pay for investment bankers and other costs associated with issuing the new stock. Since retained earnings have no such fee, the cost of new equity capital is always higher than the cost of retained earnings. Generally, the higher the floatation costs, the lower the dividend payout, given the need for equity capital in positive NPV projects.
6.   Contractual and legal restrictions - Companies may be restricted from paying dividends either by legal requirements or by implicit restrictions caused by cash needs of the business.
     -   Impairment of capital rule
     -   Debt covenants

## LOS 21.f: Calculate and interpret the effective tax rate on a given currency unit of corporate earnings under double taxation, dividend imputation, and split-rate tax systems.

Double-taxation system

![image-20211017223108553](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211017223108553.png)

Split-rate corporate tax system

The calculation of the effective tax rate under a split rate system is similar to the computation of the effective tax rate under double taxation except that the corporate tax rate applicable would be the corporate tax rate for distributed income

![image-20211018000243493](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018000243493.png)

Under an imputation tax system, taxes are paid at the corporate level but are attributed to the shareholder, so that all taxes are effectively paid at the shareholder rate.

![image-20211018000319720](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018000319720.png)

![image-20211018000329959](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018000329959.png)

## LOS 21.g: Compare stable dividend, constant dividend payout ratio, and residual dividend payout policies, and calculate the dividend under each policy.

![image-20211018000500042](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018000500042.png)

### Target payout adjustment model

![image-20211018000658312](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018000658312.png)

### Constant dividend payout ratio policy

![image-20211018000704109](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018000704109.png)

### Residual dividend model

![image-20211018000711086](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018000711086.png)

Advantages of the residual dividend model:

-   The model allows management to pursue profitable investment opportunities without being constrained by dividend considerations.

Disadvantages of the residual dividend model:

-   If a firm follows the residual dividend policy, its dividend payments may be unstable. Investment opportunities and earnings often vary from year to year.

## LOS 21.h: Compare share repurchase methods.

Four common methods are used for share buybacks, though due to varying rules, some markets may not allow all methods. Outside the United States and Canada, method 1 is used almost exclusively.

1.   Open market transactions are the most flexible approach, allowing a company to buy back its shares in the open market at the favorable terms.
2.   Fixed price tender offer is an approach where the firm buys a predetermined number of shares at a fixed price, typically at a premium over the current market price. It allows a company to buy back its shares rather quickly. If more than the desired number of shares are tendered in response to the offer, the company will typically buy back a prorated number of shares from each shareholders responding to the offer.
3.   Dutch auction is a tender offer in which the company specifies not a single fixed price but rather a range of prices. Dutch auctions identify the minimum clearing price for the desired number of shares that need to be repurchased. Each participating shareholder indicates the price and the number of shares tendered. Bids are accepted based on lowest price first until the desired quantity is filled.
4.   Repurchase by direct negotiation entails purchasing shares from a major shareholder, often at a premium over market price. This method is often used in a greenmail scenario (where a hostile bidder is offered a premium to go away) to the detriment of the remaining shareholders.

## LOS 21.i: Calculate and compare the effect of a share repurchase on earnings per share when 1) the repurchase is financed with the company's surplus cash and 2) the company uses debt to finance the repurchase.

![image-20211018003032756](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018003032756.png)

## LOS 21.j: Calculate the effect of a share repurchase on book value per share.

![image-20211018003107909](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018003107909.png)

![image-20211018003113202](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018003113202.png)

## LOS 21.k: Explain the choice between paying cash dividends and repurchasing shares.

1.   Potential tax advantages - When the tax rate on capital gains is lower than the tax rate on dividend income, share repurchases have a tax advantage over cash dividends.
2.   Share price support/signaling - Companies may purchase their own stock, thereby signaling to the market that the company views its own stock as a good investment.
3.   Added flexibility - A company could declare a regular cash dividend and periodically repurchase shares as a supplement to the dividend. Unlike dividends, share repurchases are not a long-term commitment. Since paying a cash dividend and repurchasing shares are economically equivalent.
4.   Offsetting dilution from employee stock options - Repurchases offset EPS dilution that results from the exercise of employee stock options.
5.   Increasing financial leverage

![image-20211018003404416](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018003404416.png)

![image-20211018003409746](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018003409746.png)

![image-20211018003414478](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018003414478.png)

![image-20211018003422065](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018003422065.png)

![image-20211018003451036](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018003451036.png)

![image-20211018003517189](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018003517189.png)

## LOS 21.l: Describe broad trends in corporate payout policies.

1.   A lower proportion of US companies pay dividends compared to their European counterparties.
2.   Globally, in developed markets, the proportion of companies paying cash dividends has trended downwards over the long term.
3.   The percentage of companies making stock repurchases has been trending upwards in the United States since the 1980s and in the United Kingdom and continental Europe since the 1990s.

## LOS 21.m: Calculate and interpret dividend coverage ratios based on 1) net income and 2) free cash flow.

## LOS 21.n: Identify characteristics of companies that may not be able to sustain their cash dividend.

Dividend payout ratio = dividends / net income

dividend coverage ratio = net income / dividends

![image-20211018004044901](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018004044901.png)

## LOS 22.a: Describe global variations in ownership structures and the possible effects of these variations on corporate governance policies and practices.

### Concentrated ownership vs. Dispersed ownership

Concentrated ownership, where a single shareholder or a group of shareholders have control over the corporation. These controlling shareholders can be a family, other companies, or a sovereign entity. Dispersed ownership refers to the situation where the shareholders are numerous and non has control.

Percentage ownership is not always a reliable indicator of concentration of control: certain shareholders may have a greater degree of control than their ownership percentage would suggest. A minority shareholder could have control of a corporation through a vertical ownership arrangement (where the group has a controlling interest in holding companies, which in turn have controlling interests in operating companies) or a horizontal ownership arrangement (where companies with common suppliers or customers cross-hold each other's shares).

Another disconnect between control and percentage ownership comes in the form of dual-class shares, wherein one class of shareholders has fewer voting rights, while the other class has superior voting rights.

### Conflicts within different ownership structures

Dispersed ownership and dispersed voting power describes a situation where shareholders (called weak shareholders) do not hold power over managers (called strong managers). In this situation, principal-agent conflict is likely: shareholders want shareholder value maximized, while managers may use the firm's resources to their own advantages. This problem can be mitigated by the presence of controlling shareholders.

Concentrated ownership and concentrated voting power refers to a situation where so-called 'strong' shareholders hold power over minority shareholders and 'weak' managers. This arrangement allows controlling shareholders to control the board of directors and effectively control and monitor management. The downside of this situation is that a principal-principal problem may arise: controlling owners can take advantage of firm resources to the detriment of minority owners.

Dispersed ownership and concentrated voting power indicates that the majority of the shares of a company are not owned by strong controlling shareholders. Rather, the controlling shareholders gain control over other minority shareholders through pyramid structures or dual-class shares, despite the controlling shareholders having less-than-majority ownership (again, the principal-principal problem). These controlling shareholders' voting power also allows them to monitor management.

Concentrated ownership and dispersed voting power occurs in the presence of voting caps, where the voting rights of large share positions are restricted. Sovereign countries sometimes enact voting caps to discourage foreign investors from taking a controlling position in a company belonging to an industry that is considered important.

### Categories of influential shareholders

1.   Banks - When a bank lends money to a firm or holds an equity stake, the bank can often exert some control over that corporation. (This is especially common in Asia and Europe.) The bank does not take advantage of its role as lender at the expense of other shareholders.
2.   Families - In Latin America and some other places, family ownership is common. One advantage of family control is that principal-agent issues may be reduced. On the other hand, family ownership can make it difficult to recruit quality outsiders for management and often leads to lack of concern for minority shareholders, as well as minimal transparency and low accountability by management.
3.   State-owned enterprises (SOE) - A listed SOE is partly owned by the government and also trades on an exchange.
4.   Institutional investors - In many countries, institutional investors can represent a large portion of equity ownership.
5.   Group companies - Such as South Korea's Samsung, can achieve an outsized amount of control through cross-holding of shares via vertical and horizontal ownership.
6.   Private equity firms - Introducing performance-based compensation for managers, or the addition of codes.
7.   Foreign investors - Foreign investors typically demand greater accountability and transparency. This is particularly true in emerging market countries.
8.   Managers and board directors

### Ownership structure and corporate governance

1.   Director independence - When a board member has no significant remuneration, ownership, or employment relationship with the firm, the board member is considered independent. Independent directors are important in countries with dispersed ownership where the principal-agent problem is greater and thus the board's role of monitoring mangers is key.
2.   Board structures - Under a two-tier structure, the management board is overseen by a supervisory board. This supervisory board performs functions such as determining management compensation, supervising external auditors, and reviewing the firm's financial records. In some jurisdictions, representatives of stakeholders such as labor groups sit on the supervisory board.
3.   Special voting arrangements - Some countries attempt to provide an advantage to minority shareholders through special voting arrangements for board nomination and election.
4.   Corporate governance codes, laws, and listing requirements - Some countries have adopted national 'comply or explain' corporate governance codes that require firms to either best practices of corporate governance or explain why they have not.
5.   Stewardship codes - Stewardship codes exist in some countries that seek to engage investors in corporate governance by exercising their legal rights.

## LOS 22.b: Evaluate the effectiveness of a company's corporate governance policies and practices.

When a company is not behaving according to stakeholders' wishes, shareholder activism may occur: this is the term for techniques used by shareholders to force management to act in shareholders' interests.

### Board policies and practicies

1.   Structure of board of directors - CEO duality occurs when the chairperson of the board is also the chief executive officer (CEO). CEO duality raises concerns that the chairperson's oversight and monitoring responsibilities may not be effectively rendered.
2.   Board independence - Ideally, a majority of board members should be independent; independent directors are more likely to prevent management from self-serving behavior.
3.   Board committees - Such as compensation, nomination, and audit committees. When analyzing a corporation's board, an analysts should consider whether the key committees related to financial reporting, management selection, and compensation are sufficiently independent.
4.   Skills and experience of board
5.   Composition of board - It has been observed in recent years that small, diverse boards of directors are generally more effective than large boards made up of members with similar backgrounds.
6.   Other board evaluation considerations. - A board of directors may be evaluated from a number of perspectives.

### Executive compensation

Clawback policies allow firms to reclaim past compensation if inappropriate conduct comes to light later. Say-on-pay rules can give stakeholders the opportunity to vote on executive compensation. The pay differential between the CEO and the firm's average worker has come under scrutiny in recent years.

earn-out - guarantee한 성과가 나오면 compensation을 더 주는 조항

### Voting rights of shareholders

Holding various classes of shares. Some firms structure share offerings as a single class with equal voting rights. Alternatively, in a dual-class structure, the shares held by the firm's founders or management have more voting power than hose sold to external investors.

## LOS 22.c: Describe how ESG-related risk exposures and investment opportunities may be identified and evaluated.

### Relevant ESG factors

1.   ESG data providers
2.   Industry organizations
3.   Proprietary methods - ESG data specific to a particular firm can be derived from sources such as 10-K regulatory filings, corporate sustainability reports, and annual reports.

### Security analysis: Fixed income vs. Equity

#### Fixed-Income analysis

Fixed-income analysts usually will focus on ESG factors' downside risk.

#### Equity analysis

Equity analysts consider both the upside and downside impact of ESG factors when valuing a firm's stock.

## LOS 22.d: Evaluate ESG risk exposures and investment opportunities related to a company.

### ESG integration

For example, a company's projected cash flow statements or income statement may be adjusted in terms of earnings, margins, revenues, costs, capital expenditures, or other items. Adjustments to the balance sheet often take the form of altering the value of assets of reflect impairment. The credit spread of a fixed-income instrument may be adjusted to reflect ESG concerns. Similarly, an adjustment to discount rate or cost of capital may be used to reflect ESG considerations in an equity analysis.

Green bonds are fixed-income instruments used to fund projects related to the environment.

### ESG integration examples

1.   Environment factors - Concerned about wasting water, a soft-drink company has been able to lower its water usage in its manufacturing process over the past three years.
2.   Social factors - A drug company has experienced a long string of product recalls, product quality controversies, and fines and warning letters from regulators. Negative valuation impacts for stock and bondholders are also appropriate, especially if the firm's brand reputation is impaired.
3.   Governance factors - Compared to its peers, a bank's board is found to be lagging in a number of measure: the bank's chairperson is not independent, the board's overall independence and diversity is low, board members' industry experience is low, and a number of board members have long tenures. In addition to these factors, the bank has a higher ratio of nonperforming loans than its peers. To reflect these additional risks, the analyst uses a higher risk premium to value the bank's stock and also increases the credit spread used to value the bank's debt.

## LOS 23.a: Classify merger and acquisition (M&A) activities based on forms of integration and relatedness of business activities.

![image-20211018040633506](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018040633506.png)

The terms mergers and acquisitions, or M&A for short, generally refers to two businesses combining in some manner. But almost always someone is left unhappy (usually the managers that are removed, or workers that will be laid off).

An acquisition refers to one company buying only part of another company. If the acquirer absorbs the entire target company, the transaction is considered a merger. The initiator of the venture is referred to as the bitter, or acquirer, while the opposite side of the transaction is known as the target.

### Forms of integration

#### Statutory merger

The acquiring company acquires all of the target's assets and liabilities. As a result, the target company ceases to exist as a separate entity. Note that in a statutory merger, the target company is usually smaller than the purchaser, but this is not always the case.

 흡수합병, A + B = A

#### Subsidiary merger

Acquisition

#### Consolidation

신설합병, A + B = C

### Types of mergers

#### Horizontal merger

The two business operate in the same or similar industries, and may often be competitors.

#### Vertical merger

The acquiring company seeks to move up or down the product supply chain.

Forward integration, where the acquirer is moving up the supply chain toward the ultimate consumer.

Backward integration, the company is moving down the supply chain toward the raw material inputs.

#### Conglomerate merger

다각적 인수

The two companies operate in completely separate industries.

## LOS 23.b: Explain common motivations behind M&A activity.

Synergies - Cost synergies are exactly the strategy behind a pure horizontal merger. Revenue synergies are typically created by cross-selling products, increasing market share, or raising prices to take advantage of reduced competition.

Achieving more rapid growth - External growth via M&A activity is usually a much faster way for managers to increase revenues than making investments internally (i.e., organic growth). Growth through M&A is especially common in mature industries where organic growth opportunities are limited. In addition, it is typically a less risky way to generate growth by acquiring resources through a merger with another company rather than developing them internally.

Increased market power - When a horizontal merger occurs in an industry with few competitors, the newly combined company will typically come away with increased market share and a greater ability to influence market prices. Vertical mergers may also increase market power by reducing dependence on outside suppliers.

Gaining access to unique capabilities - If a company is lacking a specific capability or resource, it can either try to develop it internally or seek to acquire something that already exists. M&A activity can be a cost effective way to acquire proven capabilities or resources.

Diversification - Managers may cite the need to diversify the firm's cash flows as grounds for a merger. This makes no sense for shareholders but may be rational for the managers. It is much easier and cheaper for the shareholders to diversify simply by investing in the shares of unrelated companies themselves rather than having one company go through the long, expensive process of acquiring and merging the two firms' operations and corporate cultures. In fact, research has revealed that conglomerates trade at a discount relative to the sum of the value of individual businesses. In this case, the whole is less than the sum of the individual parts. This finding demonstrates that mergers are not likely to increase value purely for diversification reasons.

Bootstrapping EPS - Another motivation for mergers is the bootstrapping effect on earnings per share that sometimes results from a stock deal.

Personal benefits for managers - This means that there is a strong financial incentive for managers to maximize the size of the firm rather than shareholder value. In addition, being part of the executive team for a larger company implies greater power and prestige and is probably good for managerial egos.

Tax benefits

Unlocking hidden value - When a company has struggled for an extended period of time, an acquirer may believe it can pay a lower price to buy the company and unlock hidden value by improving managements, adding resources, or improving the organizational structure.

Achieving international business goals

-   Taking advantages of market inefficiencies - Acquiring a manufacturing plant in a country where labor costs are less expensive is a prime example of gaining an advantage from an inefficient global marketplace.
-   Working around disadvantageous government policies - International M&A is a potential way to overcome barriers to free trade, such as tariffs or quotas.
-   Use technology in new markets
-   Product differenciation
-   Provide support to existing multinational clients

## LOS 23.c: Explain bootstrapping of earnings per share (EPS) and calculate a company's post-merger EPS.

Bootstrapping is a way of packaging the combined earnings from two companies after a merger so that the merger generates an increase in the earnings per share of the acquirer, even when no real economic gains have been achieved.

The 'Bootstrap effect' occurs when a high P/E firm (generally a firm with high growth prospects) acquires a low P/E firm (generally a firm with low growth prospects) in a stock transaction. Post-merger, the earnings of the combined firm are simply the sum of the respective earnings prior to the merger. However, by purchasing the firm with a lower P/E, the acquiring firm is essentially exchanging higher-priced shares of lower-priced shares. As a result, the number of shares outstanding for the acquiring firm increases, but at a ratio that is less than 1-for-1. When we compute the EPS for the combined firm, the numerator (total earnings) is equal to the sum of the combined firms, but the denominator (total shares outstanding) is less than the sum of the combined firms. The result is higher reported EPS, even when the merger creates no additional synergistic value.

![image-20211018023952955](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018023952955.png)

In practice, the market tends to recognize the bootstrapping effect and post-merger P/E's adjust accordingly. However, there have been periods in history, such as the technology bubble in the late 1990s, where bootstrapping helped high P/E companies show EPS growth, even in cases where the mergers created no value for shareholders.

![image-20211018040648612](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018040648612.png)

## LOS 23.d: Explain, based on industry life cycle, the relationship between merger motivations and types of mergers.

![image-20211018024118507](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018024118507.png)

## LOS 23.e: Contrast merger transactions characteristics by form of acquisition, method of payment, and attitude of target management.

### Forms of acquisition

-   stock purchase
    -   Finally, most stock purchases involves purchasing the entire company and not just a portion of it. This means that not only will the acquirer gain the target company's assets, but it will also assume the target's liabilities.
-   asset purchase
    -   Asset purchase acquisitions usually focuses on specific parts of the company that are of particular interest to the acquirer, rather than the entire company, which means that the acquirer generally avoids assuming any of the target company's liabilities.

![image-20211018024339238](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018024339238.png)

### Method of payment

#### Security offering

exchange ratio

The total compensation ultimately paid by the acquirer in a stock offering is based on three factors: the exchange ratio, the number of shares outstanding of the target company, and the value of the acquirer's stock on the day the deal is completed.

#### Cash offers

When an acquirer is negotiating with a target over the method of payment, there are three main factors that should be considered:

1.   Distribution between risk and reward for the acquirer and target shareholders. - In a stock offering, since the target company's shareholders receive new shares in the post-merger company, they share in the risk related to the ultimate value that is realized from the merger. In a cash offering, all of the risk related to the value of the post-merger company is borne by the acquirer. As a result, when the acquirer is highly confident in the synergies and value that will be created by the merger, it is more inclined to push for a cash offering.
2.   Relative valuations of companies involved. - If the acquirer's shares are considered overvalued by the market, the acquirer is likely to want to use its overpriced shares as currency in the merger transaction. In fact, investors sometimes interpret a stock offering as a signal that the acquirer's shares may be overvalued.
3.   Changes in capital structure. - If the acquirer borrows money to raise cash for a cash offering, the associated debt will increase the acquirer's financial leverage and risk. Issuing new stock for a securities offering can dilute the ownership interest for the acquirer's existing shareholders.

### Attitude of target management

Friendly merger offers usually begin with the acquirer directly approaching the target's management. If both parties like the idea of a potential deal, they will negotiate the method of payment and the terms of the transaction. At this point, each party to the merger will conduct due diligence on the other party by examining financial statements and other records.

Hostile merger offers

-   tender offer - the acquirer offers to buy the shares directly from the target shareholders, and each individual shareholder either accepts or rejects the offer.
-   proxy battle - the acquirer seeks to control the target by having shareholders approve a new 'acquirer approved' board of directors.

## LOS 23.f: Distinguish among pre-offer and post-offer takeover defense mechanisms.

### Pre-offer defense mechanisms

#### Poison pill

flip-in pill - where the target company's shareholders have the right to buy the target's shares at a discount

flip-over pill - where the target shareholders have the right to buy the acquirer's shares at a discount.

In case of a friendly merger offer, most poison pill plans give the board of directors the right to redeem the pill prior to a triggering event.

#### Poison put

These puts give bondholders the option to demand immediate repayment of their bonds if there is a hostile takeover. This additional cash burden may fend off a would-be acquirer.

#### Restrictive takeover laws

Historically, Ohio and Pennsylvania have been considered to provide target companies with the most protection.

#### Staggered board <-> annual election

Each group is elected for a 3-year term in a staggered system: in the first year the first group is elected, the following year the next group is elected, and in the final year the third group is elected.

![image-20211018035647856](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018035647856.png)

#### Restricted voting rights

#### Supermajority voting provision for mergers

A supermajority provision in the corporate charter requires shareholder support in excess of a simple majority. For example, a supermajority provision may required 66.7%, 75%, or 80% of votes in favor of a merger.

#### Fair price amendment

A fair price amendment restricts a merger offer unless a fair price is offered to current shareholders.

#### Golden parachutes

Golden parachutes are compensation agreements between the target and its senior management that give the managers lucrative cash payouts if they leave the target company after a merger.

### Post-offer defense mechanisms

#### "Just say no" defense

The first step in avoiding a hostile takeover offer is to simply say no. If the potential acquirer goes directly to shareholders with a tender offer or a proxy fight, the target can make a public case to the shareholders concerning why the acquirer's offer is not in the shareholder's best interests.

#### Litigation

The basic idea is to file a lawsuit against the acquirer that will require expensive and time-consuming legal efforts to right. The typical process is to attack the merger on anti-trust grounds or for some violation of securities law. The courts may disallow the merger or provide a temporary injunction delaying the merger, giving managers more time to load up their defense or seek a friendly offer from a while knight.

#### Greenmail

Essentially, greenmail is a payoff to the potential acquirer to terminate the hostile takeover attempt. Greenmail is an agreement that allows the target to repurchase its shares from the acquiring company at a premium to the market price.

#### Share repurchase

The target company can submit a tender offer for its own shares.

#### Leveraged recapitalization

In a leveraged recapitalization, the target assumes a large amount of debt that is used to finance share repurchases. Like the share repurchase, the effect is to create a significant change in capital structure that makes the target less attractive while delivering value to shareholders.

#### Crown jewel defense

After a hostile takeover offer, a target may decide to sell a subsidiary or major asset to a neutral third party. If the hostile acquirer views this asset as essential to the deal (i.e., a crown jewel), then it may abandon the takeover attempt. The risk here is that courts may declare the strategy illegal if a significant asset sale is made after the hostile bid is announced.

#### Pac-Man defense

After a hostile takeover offer, the target can defend itself by making a counteroffer to acquire the acquirer. In practice, the Pac-Man defense is rarely used because it means a smaller company would have to acquire a larger company, and the target may also lose the use of other defense tactics as a result of its counteroffer.

#### White knight defense

A white knight is a friendly third party that comes to the rescue of the target company. The target will usually seek out a third party with a good strategic fit with the target that can justify a higher price than the hostile acquirer. In many cases, the white knight defense can start a bidding war between the hostile acquirer and the third party, resulting in the target receiving a very good price when a deal is ultimately completed. This tendency for the winner to overpay in a competitive bidding situation is called the winner's curse.

대신 인수해줄 사람 찾기

#### White squire defense

The target seeks a friendly third party that bus a minority stake in the target without buying the entire company.

의결권 지원

## LOS 23.g: Calculate and interpret the Herfindahl-Hirschman Index and evaluate the likelihood of an antitrust challenge for a given business combination.

HHI (Herfindahl-Hirschman Index)
$$
\\HHI = \sum_{i = 1}^{n}{(MS_{i} * 100)^{2}}
$$
![image-20211018031151456](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018031151456.png)

![image-20211018031159064](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018031159064.png)

## LOS 23.i: Calculate free cash flows for a target company and estimate the company's intrinsic value based on discounted cash flow analysis.

## LOS 23.j: Estimate the value of a target company using comparable company and comparable transaction analyses.

Comparable company analysis uses relative valuation metrics for similar firms to estimate market value and then adds a takeover premium to determine a fair price for the acquirer to pay for the target.

![image-20211018031345117](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018031345117.png)

![image-20211018031349930](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018031349930.png)

![image-20211018031356358](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018031356358.png)

![image-20211018031402055](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018031402055.png)

### Estimate the value of a merger target using comparable transaction analysis

Comparable transactions analysis uses details from recent takeover transactions of similar companies to estimate the target's takeover value. The methodology behind the approach is very similar to the comparable company approach we just showed you, except that all of the comparables are firms that have recently been taken over. The biggest challenge is finding enough relevant takeover transactions for firms that are similar to the target being analyzed.

![image-20211018031542012](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018031542012.png)

![image-20211018031546578](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018031546578.png)

## LOS 23.h: Compare the discounted cash flow, comparable company, and comparable transactions for valuing a target company, including the advantages and disadvantages of each.

### Discounted cash flow analysis

Advantages

-   It is relatively easy to model nay changes in the target company's cash flow resulting from operating synergies or changes in cost structure that may occur after the merger.
-   The estimate of company value is based on forecasts of fundamental conditions in the future rather than on current data.
-   The model is easy to customize.

Disadvantages

-   The model is difficult to apply when free cash flows are negative.
-   Estimates of cash flows and earnings are highly subject to error, especially when those estimates are for time periods far in the future.
-   Discount rate changes over time can have a large impact on the valuation esimtate.
-   Estimation error is a major concern since the majority of the estimated value for the target is based on the terminal value, which is highly sensitive to estimates used for the constant growth rate and discount rate.

### Comparable company analysis

Advantages

-   Data for comparable companies is easy to access.
-   Assumption that similar assets should have similar values is fundamentally sound.
-   Estimates of value are derived directly from the market rather than assumptions and estimates about the future.

Disadvantages

-   The approach implicitly assumes that the market's valuation of the comparable companies is accurate.
-   Using comparable companies provides an estimate of a fair stock price, but not a fair takeover price. An appropriate takeover premium must be determined separately.
-   It is difficult to incorporate merger synergies or changing capital structures into the analysis.
-   Historical data used to estimate a takeover premium may not be timely, and therefore may not reflect current conditions in the M&A market.

### Comparable transaction analysis

Comparable transaction analysis uses details from completed M&A deals for companies similar to the target being analyzed to calculate an estimated value for the target.

Advantages

-   Since the approach uses data from actual transactions, there is no need to estimate a separate takeover premium.
-   Estimates of value are derived directly from recent prices for actual deals completed in the marketplace rather than from assumptions and estimates about the future.
-   Use of prices established by recent transactions reduces the risk that the target's shareholders could file a lawsuit against the target's managers and board of directors for mispricing the deal.

Disadvantages

-   The approach implicitly assumes that the M&A market valued past transactions accurately. If past transactions were over or underpriced, the mispricing will be carried over toe the estimated value for the target.
-   There may not be enough comparable transactions to develop a reliable data set for use in calculating the estimated target value. If the analyst isn't able to find enough similar companies, she may try to use M&A deals from other industries that are not similar enough to the deal being considered.
-   It is difficult to incorporate merger synergies or changing capital structures into the analysis.

## LOS 23.k: Evaluate a takeover bid and calculate the estimated post-acquisition value of an acquirer and the gains accrued to the target shareholders versus the acquirer shareholders.

![image-20211018040726025](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018040726025.png)

![image-20211018040733760](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018040733760.png)

![image-20211018040742138](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018040742138.png)

### Post-merger value of an acquirer

![image-20211018033745234](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018033745234.png)

### Gains accrued to the target

![image-20211018033756444](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018033756444.png)

### Gains accrued to the acquirer

![image-20211018033806574](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018033806574.png)

### Cash payment vs. stock payment

With a cash offer, the target firm's shareholders will profit by the amount paid over its current share price (i.e., takeover premium). However, this gain is capped at that amount.

With a stock offer, the gains will be determined in part by the value of the combined firm, because the target firm's shareholders do not received cash and just walk away, but rather retain ownership in the new firm. Accordingly, for a stock deal we must adjust our formula for the price of the target:
$$
\\P_{T} = N * P_{AT}
$$
![image-20211018034015970](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018034015970.png)

![image-20211018034021067](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018034021067.png)

![image-20211018034027765](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018034027765.png)

## LOS 23.l: Explain how price and payment method affect the distribution of risks and benefits in M&A transactions.

### Effect of price

This means that the acquirer will want to pay the lowest possible price (the pre-merger value of the target, $V_{T}$), while the target wants to receive the highest possible price (the pre-merger value of the target plus the expected synergies, $V_{T} + S$)

### Cash offer

In a cash offer, the acquirer assumes the risk and receives the potential reward form the merger, while the gain for the target shareholders is limited to the takeover premium.

### Stock offer

In a stock offer, some of the risks and potential rewards from the merger shift to the target firm.

The main factor that affects the method of payment decision is confidence in the estimate of merger synergies. The more confident both parties are synergies will be realized, the more acquirer will prefer to pay cash and the more the target will prefer to receive stock. Conversely, if estimates of synergies are uncertain, the acquirer may be willing to shift some of the risk (and potential reward) to the target by paying for the merger with stock, but the target may prefer the guaranteed gain that comes from a cash deal.

## LOS 23.m: Describe characteristics of M&A transactions that create value.

Short-term performance studies that look at stock returns before and after merger announcement dates conclude that targets gain approximately 30%, while acquirers lose stock value of between 1% and 3%.

Winner's curse

Managers also may overestimate the synergies and expected benefits of the merger. This tendency is called managerial hubris.

Some mergers do enhance value for the acquirer. Acquirer are likely to earn positive returns on a deal characterized by:

-   Strong buyer
-   Low premium
-   Few bidders
-   Favorable market reaction

## LOS 23.n: Distinguish among equity carve-outs, spin-offs, split-offs, and liquidation.

### Divestitures

Divestitures refer to a company selling, liquidating, or spinning off a division or subsidiary.

### Equity carve-outs

Equity carve-outs create a new, independent company by giving an equity interest in a subsidiary to outside shareholders. Shares of the subsidiary are issued in a public offering of stock, and the subsidiary becomes a new legal entity whose management team and operations are separate from the parent company.

### Spin-offs

![image-20211018040534546](/Kevin_Min/images/2021-10-17-CFA-Level-2-Corporate-Finance/image-20211018040534546.png)

Spin-offs are like carve-outs in that they create a new independent company that is distinct from the parent company. The primary difference is the shares are not issued to the public, but are instead distributed proportionately to the parent company's shareholders. This means that the shareholder based of the spin-off will be the same as that of the parent company, but the management team and operations are completely separate.

 인적분할

### Split-offs

Split-offs allow shareholders to receive new shares of a division of the parent company in exchange for a portion of their shares in the parent company. The key here is that shareholders are giving up a portion of their ownership in the parent company to receive the new shares of stock in the division.

물적분할

### Liquidations

## LOS 23.o: Explain common reasons for restructuring.

Division no longer fits into management's long-term strategy

Lack of profitability

Individual parts are worth more than the whole

Infusion of cash

