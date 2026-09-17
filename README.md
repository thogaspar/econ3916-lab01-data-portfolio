# econ3916-lab01-data-portfolio
ECON 3196 Lab 01 - The Data Portfolio 
The Data Portfolio — Big Mac Index Analysis

Objective: This project applies purchasing power parity (PPP) theory to The Economist's Big Mac Index dataset to quantify currency valuation deviations across countries and time, using panel data diagnostics to distinguish genuine economic signal from structural data artifacts.

Methodology:

Sourced raw Big Mac price data (57 countries, 45 periods spanning July 2000–July 2026) directly from The Economist's public GitHub repository
Constructed implied PPP exchange rates from local Big Mac prices and computed each currency's percentage valuation against the US dollar
Classified the dataset's structure across its three natural dimensions — cross-sectional (single-period, 54-country snapshot), time-series (single-country trajectories), and full panel (country × period)
Conducted a missing-data audit on the unbalanced panel, diagnosing Russia's exit from the sample as Missing Not At Random (MNAR), tied to its 2022 removal following sanctions rather than to any random data-collection failure
Built two complementary visualizations: a cross-sectional bar chart ranking current currency valuations, and a time-series comparison tracking selected countries' deviations across the full sample period

Key Findings:

The Swiss franc emerged as the most persistently overvalued currency in the sample, trading +41.8% above PPP-implied fair value in the July 2024 cross-section
The Japanese yen showed the opposite pattern: undervalued on average in every decade of the 2000–2026 series, consistent with a sustained structural gap between Japanese Big Mac prices and dollar-converted fair value
The missing-data diagnosis underscores a broader methodological point: naively dropping incomplete country panels (e.g., Russia) would not produce a random subsample — it would selectively remove politically driven exits, biasing any full-panel PPP averages
