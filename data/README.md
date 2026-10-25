# NSW coastal safety data (for Data Visualisation 2)

## Source
National Coastal Safety Report 2025, Surf Life Saving Australia (October 2025), NSW pages 68 to 71 and 74 to 75.
Covers 2024/25 (1 July 2024 to 30 June 2025) unless the file says otherwise.

## Files
- nsw_coastal_drownings_by_year.csv: coastal drowning deaths per year, 2015/16 to 2024/25 (from the Figure 73 bar labels)
- nsw_coastal_drownings_by_branch.csv: deaths and average rate per 100,000 by SLSNSW branch, 2015 to 2025 (page 71)
- nsw_rescues_2024_25.csv: rescues by craft or method, 2024/25 (page 68)
- nsw_coastal_drowning_profile_2024_25.csv: percentage breakdowns for 2024/25 (page 69)

## Known discrepancies in the source (check before publishing)
- 2024/25 rate is 0.63 per 100,000 on page 69 but 0.61 on page 70.
- Branch deaths total 453, but the yearly counts total 471 for the same 10 years.
- The stated 10-year average is 46, but the yearly counts average 47.1.
- Cite the page number when you use any of these figures, and mention the discrepancy in your description if you show the totals.

---

# National data (second source)

## Source
Royal Life Saving Society - Australia, National Drowning Report 2025 (August 2025), https://doi.org/10.62977/118009
Covers 1 July 2024 to 30 June 2025 unless the file name says otherwise. PDF page numbers are given below.

## Files
- aus_drowning_by_state_2024_25.csv: deaths, 10-year average, rates and change by state (pages 62 to 63 and state pages 66 to 95). States sum to 357, matching the national total.
- aus_top_regions_drowning_rate.csv: top 10 regions and top 10 metro regions by residential drowning rate, 2014/15 to 2024/25 (page 64)
- aus_drowning_by_age_2024_25.csv: rate and share of deaths by 5-year age group (page 11)
- aus_coastal_drowning_by_age_2020_25.csv: coastal deaths by age, 2020/21 to 2024/25 (page 47)
- aus_coastal_drowning_by_birth_continent_2020_25.csv: coastal deaths by continent of birth, 2020/21 to 2024/25 (page 47)
- aus_coastal_drowning_by_activity_2020_25.csv: coastal deaths by activity, 2020/21 to 2024/25 (page 49)
- aus_coastal_drowning_by_month_2020_25.csv: coastal deaths by month and season, 2020/21 to 2024/25 (page 49)

## Notes and discrepancies
- ACT shows "<5" on the state map (page 63) but the ACT page says 1 death. The CSV uses 1.
- Tasmania's rate of 1.39 is labelled "2023/24" on its state page, but the text says 2024/25. The CSV treats it as 2024/25.
- Percentages are rounded in the report, so some groups sum to 98 to 101.
- The coastal age file keeps "<1" as text for two groups. Treat it as a small value, not zero.
- Rates marked yes in fewer_than_10_cases are flagged by the report as "interpret with caution".
- Regional rates are by where people lived, not where they drowned.

## Added for the flow map
- coastal_birth_flows.csv: the continent-of-birth percentages from aus_coastal_drowning_by_birth_continent_2020_25.csv, with a representative origin point for each continent and a destination point in Australia, placed by the author. Australia (41%) and Unknown (22%) are not drawn as lines.
- world-110m.json: world basemap (TopoJSON), Natural Earth via vega-datasets, https://github.com/vega/vega-datasets
