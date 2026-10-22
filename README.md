# Call Center Operations Dashboard

Excel analysis of 200,000 call records from 2024, covering recorded outcomes, abandonment, discussed products and agent workload.

![Call Center Operations dashboard](dashboard.png)

[Download the workbook](Call_Center_Operations_Dashboard.xlsx)

## Results

- Recorded success represents 41.76% of all calls and 53.76% of non-abandoned calls.
- There are 44,644 abandoned records, or 22.32% of all calls.
- Long Wait Time is recorded on 42,160 abandoned calls, representing 94.44% of abandoned records.

The dashboard combines a monthly outcome-mix chart, ranked product volumes, abandonment reasons and an agent comparison with conditional formatting. The reason distribution makes queue access worth investigating with actual waiting-time and routing data.

## Workbook

**Call Review** has the dashboard month selector. **Daily Report** has an independent month selector. **Period Analysis** contains weekly through annual summaries for 2024. **Call Metrics** holds calculations, **Data Quality** contains profiling and reconciliation checks, and **Dataset** contains the operational records.

Calculations use COUNTIFS, SUMIFS, AVERAGEIFS, IF, INDEX/MATCH and date functions. Charts are native and editable. The monthly outcome chart always shows the full year; the dashboard selector changes the KPI, product, reason and agent comparisons.

## Definitions

Each source row counts once. The original Call_ID contains only 13 repeated labels and is not a unique event key. Success plus Failure forms the non-abandoned denominator. Success is a source outcome label, not verified sales revenue.

Average duration excludes 44,644 missing observations. Product comparisons use records with a discussed product. Reason analysis filters to abandoned calls before combining capitalization variants. Follow-up flags indicate requirements, not completion or overdue work. Agent comparisons do not adjust for call mix or routing.

The public workbook excludes customer names, age, gender, state and income. RecordNo retains source row order; supplied originals remain unchanged locally.

## Refresh

Open in Excel with Automatic calculation. Append operational records inside the **CallData** table, keeping dates numeric and headers unchanged. New agents, products or years need the displayed lists or calendar extended. Weeks start on Monday; partial weeks are excluded from growth comparisons. There is no external-file refresh connection.

Totals, duration denominators, reason filters, selectors, period reconciliations and saved chart/formula references were checked. The operational source and existing metric formulas were preserved in this redesign. Desktop Excel recalculation remains unverified.
