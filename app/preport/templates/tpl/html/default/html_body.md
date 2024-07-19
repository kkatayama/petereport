# {% translate "Document Overview" %}

{{DB_report_query.product.description | safe }}

# {% translate "Executive Summary" %}

{{DB_report_query.executive_summary | safe_markdown | bleach}}

## {% translate "Summary of Findings Identified" %}

<div class="chart">
<center>
  <div id="SeveritybarChartEcharts" style="width:80%; height:450px;"></div>
</center>
</div>

{{finding_summary_table}}

## {% translate "Scope" %}

### {% translate "In Scope" %}

{{DB_report_query.scope | safe_markdown | bleach}}

### {% translate "Out of Scope" %}

{{DB_report_query.outofscope | safe_markdown | bleach}}

## {% translate "Methodology" %}

{{DB_report_query.methodology | safe_markdown | bleach}}

## {% translate "Recommendations" %}

{{DB_report_query.recommendation | safe_markdown | bleach}}

# {% translate "Findings and Risk Analysis" %}

{{template_findings}}

{{template_appendix}}
