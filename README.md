# AI Development Globalization and Multinational Enterprises' Performance

## Overview

As multinational enterprises (MNEs) race to modernize, they face a critical strategic dilemma: does expanding Artificial Intelligence across every global market actually pay off? While AI promises to make global supply chains hyper-responsive to local market shifts, attempting to manage it across dozens of countries introduces a layer of operational complexity that can silently erode profits. In this research, I address this tension by studying the impact of **AI Development Globalization** on foreign profitability. I theorize a trade-off: while expanding AI globally sharpens a firm's ability to sense and act quickly, stretching these capabilities too broadly creates an information overload that outweighs the benefits.

## Data and Method

My analysis draws on a combination of financial data from Compustat and a rare proprietary dataset that captures the presence of AI development technologies. The dataset comprises **+700 million observations across 57 countries**. I focused on Fortune 1000 firms because they are more likely to be publicly traded and disclose financial data. **AI Development Globalization** is measured at the firm level, reflecting the proportion of countries where each firm reported using at least one AI technology in any of its business units.

To ensure the robustness of the results, I employed two rigorous econometric strategies to isolate the causal impact of technology on foreign profits:

1.  **Two-Way Fixed-Effects Model:** Utilized to control for unobserved firm-specific characteristics and time-varying global shocks, while independent variables were lagged by one year to strictly establish temporal precedence.
2.  **Arellano-Bond (System GMM) Dynamic Panel Estimator:** Implemented to address endogeneity concerns, specifically the dynamic nature of profitability and simultaneity bias where profitable firms might simply invest more in technology. This method modeled profit persistence by including three lags of the dependent variable and utilized lagged levels of endogenous regressors as instruments, the validity of which was confirmed via the Hansen J test for overidentifying restrictions.

## Results

I find an inverted U-shaped relationship between **AI Development Globalization** and globalization performance, meaning firms implementing **AI Development Globalization** either too narrowly or too broadly experienced lower foreign profitability. These results imply that **AI Development Globalization** is beneficial to an MNE's foreign profit until a certain level, beyond which the marginal effects are negative.

### Main Results: Impact on Foreign Profit

**Table 1: Two-Way Fixed Effects and Dynamic Panel Models**

| Variable | (4) FE Foreign Profit | (5) Arellano-Bond Foreign Profit |
| :--- | :--- | :--- |
| **AI Development Globalization** | **20.287\*\*\*** (7.826) | **25.391\*\*** (11.883) |
| **AI Development Globalization Sq.** | **-0.265\*\*** (0.105) | **-0.334\*\*** (0.144) |
| **Big Data Globalization** | **-7.180\*\*** (3.626) | **-18.971\*** (10.184) |
| **Big Data Globalization Sq.** | **0.100\*\*** (0.047) | **0.211\*\*** (0.107) |
| **SGA** | -16.619 (12.563) | -7.868 (18.349) |
| **RD** | -100.466 (74.275) | 14.449 (51.395) |
| **Size** | 123.982 (130.026) | -41.722 (170.820) |
| **Age** | -140.534 (94.845) | 3.558 (15.190) |
| **Competition** | 311.601 (611.141) | 640.437* (358.804) |
| **Density** | -3.041 (4.486) | -0.349 (1.211) |
| **Tobin's Q** | 124.991** (62.010) | 72.768 (60.738) |
| **Foreign Profit (t-1)** | | 0.544*** (0.085) |
| **Foreign Profit (t-2)** | | -0.469** (0.185) |
| **Foreign Profit (t-3)** | | 0.837*** (0.221) |
| **Observations** | 2,986 | 1,638 |
| **Number of Firms** | 452 | 431 |

*Standard errors in parentheses. \*\*\* p<0.01, \*\* p<0.05, \* p<0.1*


**Figure 1: Predictive Values of Foreign Profits at Different Values of AI Development Globalization.**
<img src="docs/images/AIDG.jpg" width="600" alt="Predictive Values of Foreign Profits at Different Values of AIDG">

