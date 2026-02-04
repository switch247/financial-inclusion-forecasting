Interim Report: Financial Inclusion Forecasting System (Ethiopia)
Client: Consortium of Development Finance Institutions, Mobile Money Operators, and National Bank of Ethiopia (NBE)
Consultancy: Selam Analytics
Date: February 3, 2026
1. Business Objective and Context
1.1 Objective
The primary objective of this project is to develop a robust financial inclusion forecasting system for Ethiopia. By leveraging historical survey data, regulatory reports, and event-based markers, Selam Analytics aims to provide the consortium with actionable forecasts for two primary pillars of the Global Findex Framework:
Access (Account Ownership Rate): The percentage of adults (15+) with an account at a bank or other financial institution, or with a mobile money provider.
Usage (Digital Payment Adoption Rate): The frequency and breadth of digital financial services, specifically focusing on mobile money and P2P transfers.
1.2 Context: Ethiopia’s Digital Transformation
Ethiopia is currently at a critical inflection point in its financial history. Since the launch of Telebirr in 2021 and the entry of M-Pesa in 2023, the landscape has shifted from cash-dominant to digital-first. A major milestone was recently reached where interoperable P2P digital transfers surpassed ATM cash withdrawals. However, a gap remains: while digital usage is exploding, the 2024 Global Findex survey reported only a 49% account ownership rate—a modest 3% increase since 2021. This report investigates this "adoption-ownership" gap to forecast trajectories for 2025–2027.
2. Completed Work: Data Exploration and Enrichment (Task 1)
2.1 Unified Schema and Data Quality
We successfully implemented a Unified Schema consisting of:
Observations: Quantitative historical data (e.g., % account ownership).
Events: Qualitative milestones (e.g., M-Pesa launch).
Impact Links: Relationships mapping events to specific indicators with lag times.
Targets: Strategic goals set by the National Bank of Ethiopia.
Data Quality Assessment: Our audit revealed a "fragmented frequency" issue. Global Findex indicators are updated every 3 years, while Mobile Money data is available monthly. This necessitates interpolation and proxy indicators for forecasting.
2.2 Data Enrichment
We enriched the dataset with:
Macro-Economic Indicators: Inflation and GDP growth.
Regulatory Milestones: NFIS-II policy updates.
Infrastructure: 4G/LTE footprint data.
3. Exploratory Data Analysis (Task 2)
3.1 Insight 1: Account Ownership Trajectory
The data confirms a significant slowdown in account ownership growth (46% in 2021 to 49% in 2024). This suggest a "Saturation of the Urban Elite," where expansion into rural areas is the next major hurdle.
[account_ownership_rate_over_time.png] 

description: Time series of account ownership rate showing the growth trajectory and the recent 2021-2024 slowdown.
3.2 Insight 2: Source Type Diversity
To bridge the gap between triennial survey data and high-frequency market changes, our unified dataset integrates various source types. This mix allows us to use reports and news as leading indicators for the more formal survey-based Access metrics.


description: Bar chart showing the distribution of records by source type (survey, report, news, etc.), highlighting the multi-dimensional nature of the dataset.

3.3 Insight 3: Mobile Money Growth
While total account ownership is slow, mobile money accounts specifically have surged, indicating a migration from traditional banking to digital wallets.

description: Time series of mobile money account rate showing its increasing share in the financial landscape.
3.4 Insight 4: Data Distribution by Pillar
Our analysis shows that the majority of our enriched data currently falls under the "Usage" pillar, reflecting the higher frequency of reporting for mobile money metrics compared to traditional "Access" metrics.
description: Bar chart showing the distribution of records by pillar (access, usage, etc.), illustrating the data density for each area.
3.5 Insight 5: Data Confidence and Reliability
The reliability of our forecasting will depend on data confidence. Currently, a significant portion of event-based data is categorized as "Medium" confidence.

description: Bar chart of record counts by confidence level, providing a quality assessment of the underlying dataset.
4. Next Steps and Key Areas of Focus
4.1 Task 3: Event Impact Modeling
We will build an Event-Indicator Association Matrix to weight how much specific policy changes or product launches contribute to inclusion. We will test this against the 2021 Telebirr launch for calibration.
4.2 Task 4: Forecasting (2025–2027)
We will employ ARIMA and Exponential Smoothing models supplemented by event-based impact links, including:
Uncertainty Quantification: Providing 80% and 95% confidence intervals.
Scenario Analysis: Modeling "Best-Case" vs. "Status Quo" scenarios.
4.3 Task 5: Dashboard Development
The final deliverable will be an interactive dashboard to toggle events and visualize the "Gap to Target" for NBE's strategic objectives.
4.4 Data Limitations & Hypotheses
Limitation: Lack of gender-disaggregated monthly data.
Hypothesis: Rural mobile money adoption is the primary driver for meeting 2027 targets, rather than urban banking expansion.


