# Reading the Bike Company report

Open **Bike Company.pbix**. The nine-page report connects overall performance, growth, product economics, markets and customer coverage. Use the bottom navigation to follow the story; Ctrl+click in Desktop edit mode.

## What the comparison shows

All-data baseline, 1 July 2017–15 June 2020; USD. Profit means gross profit using the supplied standard costs.

| Bike family | Revenue | Gross profit | Gross margin | Units | Revenue / unit | Cost / unit | Gross profit / unit |
|---|---:|---:|---:|---:|---:|---:|---:|
| Road | $43,947,796.74 | $4,433,908.49 | 10.09% | 47,148 | $932.12 | $838.08 | $94.04 |
| Mountain | $36,622,296.45 | $6,109,768.65 | 16.68% | 28,321 | $1,293.11 | $1,077.38 | $215.73 |
| Touring | $14,545,073.65 | $466,060.10 | 3.20% | 14,751 | $986.04 | $954.44 | $31.60 |

Road bikes lead revenue and volume. Mountain bikes generate more gross profit, with roughly 2.29 times road bikes' gross profit per unit. Touring bikes have a narrow $31.60 average unit spread. These are observed product-mix outcomes, not estimates of what would happen if sales were shifted between categories.

## The model-level explanation

- **Mountain-200** generates $4,962,802.67 gross profit at 22.25% margin, a major contributor to mountain bikes' performance. Protect its economics and assess capacity and demand before scaling.
- **Touring-3000** loses $107,428.96 overall. Its average revenue per unit ($442.63) is below its standard cost ($461.44), a negative spread of $18.82 across 5,709 units.
- Touring-3000's identified-customer transactions generate $151,688.81 gross profit on 540 units at $742.35 revenue per unit. Unassigned-customer transactions lose $259,117.77 on 5,169 units at $411.32 revenue per unit. These groups describe customer-key coverage. The data does not establish that unassigned transactions belong to any particular sales channel.
- Touring-3000 loses $146,668.00 in 2019 and earns $39,239.03 in the available 2020 period. 2020 ends on 15 June; these are not comparable full-year totals. The annual split prevents treating the historical loss as a uniform current condition.
- Its US and Canadian gross losses are $71,399.32 and $26,476.98. Australia is positive at $13,708.21. Review contracts, transaction prices, product mix and cost policy; geography alone is not a demonstrated cause.
- **Road-650** and **Road-450** also have negative aggregate gross profit: $14,138.85 and $21,985.25 respectively. Review their realized pricing against standard cost.

## Components

Components generate $11.80M revenue and $1.04M gross profit at 8.79% margin. Mountain frames contribute $488,640.55 gross profit. Road frames have only 3.62% margin. Touring frames lose $2,967.04, split across HL Touring Frame ($2,872.49 loss) and LL Touring Frame ($94.55 loss). Wheels have 25.89% margin. A margin opportunity does not prove customer demand; use targeted tests for relevant parts bundles.

## How to explore the report

1. On **03a Bike comparison**, compare the three illustrated bike families. Year and country filters update the cards and the gross-profit-per-bike chart.
2. In the Components model matrix, right-click a model row and choose **Drill through → 03c Product detail**.
3. Inspect price versus cost by market and gross profit by year.
4. Use the native Back arrow to return from drill-through. In Power BI Desktop editing mode, buttons may require Ctrl+click.
5. Alternatively, open **03c Product detail** and choose a model from its slicer. All shows combined economics; choosing a model narrows the cards and charts.
6. On **03b Components**, inspect the low-profit component models and compare component-family margins.

## Validation and limits

The bike and component model totals reconcile to their category totals within one cent. Touring-3000's unit-price/cost/profit arithmetic and customer-coverage split reconcile. No sales lines have a standard cost differing from the related product standard cost by more than one cent. This verifies internal consistency, not the accounting validity or historical accuracy of the cost policy. No source refresh was performed.

Aggregate checks and reconciliation results are retained in the local working folder. The Touring-3000 callout on Bike comparison is an all-data baseline. The full development scripts and earlier report versions remain in the local working folder.

## Illustrations

Created with the built-in Image Generation tool and embedded locally. They represent bike categories, not the specific named models in the sales data:
- assets/road-bike.png
- assets/mountain-bike.png
- assets/touring-bike.png

Shared final prompt: Use case: product-mockup. Asset type: individual bike category illustration for a Power BI business report. [Subject below.] Premium photorealistic studio product photograph, exact side profile, complete bike centered fully within frame with generous margins, wheels fully visible, mechanically plausible frame and drivetrain. Seamless very light warm gray studio background, soft subtle ground shadow. Wide landscape 3:2 composition. No people, text, numbers, logos, watermarks or extra objects. Consistent clean commercial catalog lighting. This is category illustration, not an image of an actual named model from a sales dataset.

Road subject: An unbranded graphite road bicycle with slim tires, drop handlebars, compact racing geometry, and subtle teal accents.
Mountain subject: An unbranded graphite hardtail mountain bicycle with wide knobby tires, front suspension fork, flat handlebars, and subtle teal accents.
Touring subject: An unbranded graphite touring bicycle with relaxed geometry, drop handlebars, fenders, rear cargo rack with two small panniers, and subtle teal accents.
