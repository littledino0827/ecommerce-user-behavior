# E-commerce User Behavior & Conversion Analysis

## Overview
This project conducts an end-to-end analysis of user behavior on a multi-category e-commerce platform, with a focus on understanding the **view → cart → purchase** conversion funnel.  
The objective is to identify where users drop off, how behavior varies across segments, and which intervention points would generate the highest impact on purchases.

The analysis is framed from a **product and business decision-making perspective**, emphasizing metrics definition, segmentation, and impact-based prioritization rather than predictive modeling.

---

## Key Questions
- How do users interact with the platform at a high level?
- Where does the primary conversion drop-off occur in the funnel?
- How do conversion patterns vary across categories and price tiers?
- Which funnel step should be prioritized to maximize purchase uplift?

---

## Data & Methodology
- Event-level behavioral data including `view`, `cart`, and `purchase`
- Session- and user-level aggregation to construct conversion funnels
- Category and price-tier segmentation
- Scenario-based impact analysis to assess marginal gains from improving specific funnel steps

All analysis is performed using **Python and SQL (DuckDB)**.  
Raw data files are not included in this repository.

---

## Key Findings
- The platform exhibits heavy browsing behavior, with most sessions not progressing beyond views.
- A small subset of high-intent sessions accounts for the majority of purchases.
- The largest conversion drop-off occurs between **view and cart**, indicating friction at the consideration stage.
- Conversion efficiency varies significantly across categories and price tiers.
- Improving the **view-to-cart** step yields the highest marginal impact on total purchases.

---

## Business Implications
- Funnel optimization should prioritize reducing friction before cart addition rather than post-cart interventions.
- Category-specific strategies are likely more effective than one-size-fits-all optimizations.
- Behavioral segmentation provides a foundation for targeted product and UX experiments.

---

## Limitations & Next Steps
- The analysis is observational and not based on controlled experiments.
- Causal interpretation is limited by the absence of A/B testing and external user attributes.
- Future work could incorporate experimentation data, marketing exposure, or personalization signals.

---

## Tools
Python · SQL (DuckDB) · pandas · Jupyter Notebook
