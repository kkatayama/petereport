{% load martortags %}
{% load bleach_tags %}
{% load i18n %}
---
title: "{{DB_report_query.title| safe | bleach}}"
product: "{{DB_report_query.product.name| safe | bleach}}"
author: ["{{md_author}}", "Report ID: {{DB_report_query.report_id| safe | bleach}}"]
date: "{{report_date}}"
subject: "{{md_subject}}"
subtitle: "{{DB_report_query.report_id}}"
website: {{md_website}}
counter_finding_critical: "{{counter_finding_critical}}"
counter_finding_high: "{{counter_finding_high}}"
counter_finding_medium: "{{counter_finding_medium}}"
counter_finding_low: "{{counter_finding_low}}"
counter_finding_info: "{{counter_finding_info}}"
lang: "en"
colorlinks: true

---
