# Subscription Paywall A/B Test Analysis

## Overview

Analysis of an A/B test evaluating a redesigned subscription paywall for a mobile freemium photo editing application. The objective was to assess the impact of the new design (Variant B) on conversion rate and revenue per visitor, and to support a product decision on rollout.

The experiment ran over a 19-day period with approximately 892K paywall visits.

---

## Business Context

The application operates on a freemium model where users access core editing functionality for free, while premium features require a paid subscription. A new paywall design was introduced to improve monetization performance.

Variants:

* Variant A: Existing paywall design
* Variant B: Redesigned paywall with updated pricing layout and copy

---

## Data

Dataset: `ab_dataset.csv`

Access: [https://drive.google.com/drive/folders/11Pot7T024qTnTVWsyqjn_QzaDA5yTwaR?usp=sharing]

---

## Data Quality

* Duplicate visit-level records were identified and removed
* No cross-variant assignment inconsistencies detected
* Minor data correction applied for invalid conversion-revenue pairing
* Final dataset: ~887K valid records
* Balanced assignment across variants (~50/50)

---

## Conclusion

No statistically significant improvement was observed in either conversion rate or revenue per visitor.

While Variant B shows positive directional signals, particularly in higher-tier revenue distribution, the effect is not stable or strong enough to support a full rollout decision under the current evidence.

---

## Recommendation

Variant B should not be shipped based on current results. The observed uplift is small, inconsistent over time, and not statistically reliable.

Further testing is recommended with:

* Larger sample size to improve statistical power
* Separation of pricing layout vs messaging changes
* Additional segmentation analysis to identify high-value user groups

---

## Limitations

* Short observation window (19 days)
* High variance and zero-inflated revenue distribution
* Limited ability to detect small effect sizes
* Changes in traffic composition during the experiment
* No external attribution or acquisition context included

---

## Future Work

* Higher-powered follow-up experiment
* Pricing strategy isolation tests
* User segmentation (platform, geography, acquisition source)
* Long-term retention impact evaluation
* Sequential or multi-armed testing approaches

---

## Author

Erik Shahbazyan
