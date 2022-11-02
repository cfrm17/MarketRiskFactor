# Market Risk Factor Selection

The identification and selection of market risk factors to be captured in a risk model, such as VaR, are critical to building strong risk measurement platform. Risk factors are market variables which are expected to impact valuation P&L. In VaR, “risk factors” also define the returns which are simulated and subsequently mapped to market instruments. Generally, risk factors should:

·         Be related to the market instruments resulting in P&L
·         Provide strong explanatory power for P&L
·         Offer an effective method for profit attribution

Risk factors in the VaR model define the parameters which are simulated in the Monte Carlo engine. The starting point for defining risk factors is reviewing the pricing models market parameters. These market factors and inputs are candidates to be included as risk factors to VaR. The inclusion of risk factors will be chosen to minimize the Unexplained P&L (see Unexplained P&L section below). The inclusion of risk factors also requires the generation of sensitivities (to which simulated returns are to be applied) and market data for calibration.

Risk factor granularity includes the selection of points along a curve or surface that are simulated in VaR. In many cases, the selection of these points will be dependent on the tradable instruments that desks have been authorized to trade. For example, a desk authorized to trade bond instruments with a final maturity of 10y will have interest rate sensitivity to various tenor points up to 10years. Thus the selection of risk factors should include instruments having up to 10years in maturity. 

The selection of factors may require an evaluation of the simulation modelling under various definitions (such as simulating relative or absolute returns). To the extent that not all market inputs for valuation are represented in the VaR risk factor simulation set, this should be investigated and the justification documented. Often market inputs are rendered more coarse as they are translated to risk factors (i.e. a 27 point yield curve for valuation may be translated to a 5 point yield curve for VaR simulation). Such translations should also be reviewed and documented as to evidence that the underlying characterization of the market risk is preserved.

With a semi-annual frequency, factors used to decompose P&L for PAA purposes should be compared to risk factors simulated in VaR. PAA involves either 1) a greek-based approach which incorporates changes in PAA market inputs and PAA Greeks or 2) a full revaluation, sequential perturbation of PAA market inputs. This comparison will be facilitated through common pricing model.

For PAA approach #1, the collection of PAA Greeks should be compared against the VaR Greeks. For example, PAA for an equity derivatives desk may employ an equity ‘delta’ or risk sensitivity to equity price changes. The suite of VaR Greeks should also contain this term. Similarly, PAA market inputs should be compared with VaR Risk Factors. For example, if equity price changes are part of the PAA process, they should also be simulated in VaR. To the extent that these comparisons yield differences, an investigation should be launched.

For PAA approach #2, the PAA Market Inputs should be compared with the VaR Risk Factors. For example, for a given LOB, the monthly PAA should be reviewed and material contributors should be investigated to ascertain key PAA Market Input drivers. These items should then be confirmed as part of the VaR simulation. To the extent that these comparisons yield differences, an investigation should be launched.

The list of risk factors will evolve over time depending on the relevant market data, portfolio holdings or other parameters. For new products, a review of the required risk factors against existing risk factors will occur as part of the IAAP process. Risk factors that are not simulated in VaR will need to be added to the risks not in VaR list as part of the Risk Measurement Completeness Review.

Bond yield or bond spread can be used as bond risk factors. See https://finpricing.com/lib/FiZeroBond.html
