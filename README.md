# Call Center Operations Dashboard

Excel analysis of 200,000 call records from 2024, covering outcomes, abandonment, discussed products and agent workload.

![Call Center Operations dashboard](dashboard.png)

[Download the workbook](Call_Center_Operations_Dashboard.xlsx)

## Results

- Recorded success represents 41.76% of all calls and 53.76% of non-abandoned calls.
- There are 44,644 abandoned records, or 22.32% of all calls.
- Long Wait Time is recorded on 42,160 abandoned calls: 94.44% of abandoned records.

The dashboard opens at 100% zoom. It combines top-five agent volumes plus the remaining agents, an outcome doughnut, stacked product outcomes, abandonment-reason bars and a monthly call trend with highlighted minimum/maximum points. The reason distribution suggests investigating queue access using actual waiting-time and routing data.

## Workbook

**Call Review** has a month selector. **Daily Report** has an independent month selector. **Period Analysis** contains weekly through annual summaries. **Call Metrics** contains calculations, **Data Quality** contains reconciliation checks, and **Dataset** contains the operational records.

Calculations use COUNTIFS, SUMIFS, AVERAGEIFS, IF, INDEX/MATCH and date functions. All five dashboard charts are native and editable. The monthly trend always shows 2024; the dashboard selector updates KPIs, outcomes, products, reasons and agent volumes.

## Definitions

Each source row counts once. The original Call_ID contains 13 repeated labels and is not a unique event key. Non-abandoned calls comprise Success plus Failure. Success is a recorded outcome, not verified sales revenue.

Average duration excludes 44,644 missing observations. Product comparisons include records with a discussed product; abandoned calls have no recorded product. Reason analysis filters to abandoned calls before combining capitalization variants. Follow-up flags indicate requirements, not completed or overdue work. Agent volumes are descriptive and do not measure effectiveness or adjust for call mix.

The public workbook excludes customer names, age, gender, state and income. RecordNo preserves source row order. Supplied originals remain unchanged locally.

## Use

Open in Excel with Automatic calculation. Append operational rows inside **CallData**, retaining headers and numeric dates. Extend lists or calendar for new agents, products or years. Weeks start on Monday; growth comparisons exclude partial weeks. There is no external-file refresh connection.

Source values, metric formulas, chart caches, denominators, report reconciliations and saved 100% zoom were checked. Both the complete workbook and its charts were opened in Desktop Excel without a recovery warning.
