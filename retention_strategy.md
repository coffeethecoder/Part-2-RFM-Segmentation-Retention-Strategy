# Retention Strategy

## Segment Logic
- Champions: low recency, high frequency, high spend.
- Loyal but at risk: good monetary history but stale recency and low recent sessions.
- Discount hunters: high average discount and low full-price purchase share.
- Support-stressed: recent support tickets with negative sentiment.
- Dormant: high recency and zero sessions in the last 30 days.
- Maintain: customers without urgent risk signals.

## Segment Summary
| segment_name | customers | churn_rate | avg_recency | avg_frequency | avg_monetary | avg_campaign_cost |
| --- | --- | --- | --- | --- | --- | --- |
| Loyal but at risk | 111 | 0.8919 | 187.84 | 4.9369 | 4,157.67 | 17.6396 |
| Dormant | 53 | 0.8491 | 206.53 | 2.0189 | 1,458.11 | 18.5660 |
| Discount hunters | 542 | 0.5314 | 88.9133 | 2.4834 | 1,573.87 | 18.0443 |
| Maintain | 1176 | 0.4881 | 96.7194 | 3.0119 | 2,292.09 | 18.7560 |
| Support-stressed | 231 | 0.4286 | 46.6017 | 3.1991 | 2,522.37 | 17.6667 |
| Champions | 287 | 0.0767 | 18.1463 | 6.4634 | 5,049.44 | 19.0348 |

## Budget Prioritization
Use `last_campaign_cost` and `manual_priority_bucket` as the baseline to compare against. With a limited campaign budget, prioritize `Loyal but at risk` and `Support-stressed` customers first, because their churn appears more preventable than fully dormant low-engagement customers. `Discount hunters` should receive margin-safe bundle offers, not blanket discounts. `Champions` should get loyalty recognition rather than expensive save offers.
