1. Dataset Overview
Rows: 3008

Columns: 6 (index, Format, Metric, Year, Number of Records, Value (Actual))

Time Range: 1973 – 2019

Formats: 24 (examples: CD, DVD Audio, Ringtones & Ringbacks, Cassette, Vinyl Single, Paid Subscription)

Metrics: Units, Value, Value (Adjusted)

Only ~1351 rows have non-null Value (Actual) — meaning lots of missing values for some year/format/metric combinations.

2. Yearly Analysis
You computed yearly averages:

Top early years for average Value (Actual):

1978: ~1619

1977: ~1459

1979: ~1330

1981: ~1213

1980: ~1211

Trend plot (plt.plot): You plotted Value (Actual) vs Year showing sharp increases during late 70s and 80s, then fluctuations with eventual decline in certain metrics.

3. Format-Based Analysis
Most frequent formats in dataset: CD, DVD Audio, Ringtones & Ringbacks (~141 each)

Total Value by Format:

text
CD                 525,411
Cassette           157,208
LP/EP              127,648
Download Single     45,894
Paid Subscription   42,514
Vinyl Single        22,055
… many niche formats have smaller totals (like SACD, Kiosk)

4. Metric Trends
Maximum Value (Actual) by Metric:

Units: ~1,402

Value: ~13,214

Value (Adjusted): ~19,667

5. Statistical Distribution
You used a boxplot for first 200 rows:

Big variation in values for the same formats

Outliers likely correspond to peak-selling years for popular formats (e.g., CD in its boom years)

6. Pivoted Year-Metric Data
You created a groupby table with Year vs three metrics (Units, Value, Value Adjusted).
Observations:

Units plateau in the 80s–90s, peak in the late 90s (~1160 units average), decline post-2000

Value Adjusted rises sharply mid-80s to late-90s, peaks around 1999–2000, then falls significantly

Value (actual dollars) peaks in 1999–2000; digital formats rise post-2010 but don't offset physical drop

7. Visual Trends
From your seaborn/matplotlib plots:

Barplot (yearly_avg) shows clear growth from late 70s → peak mid-late 90s → decline

Line plot (Value over time) shows volatility but strong 80s–90s dominance

Boxplot reveals wide dispersions in format revenues — supporting the idea of a few dominant formats

Overall Insight
Physical formats (CD, Cassette, LP) dominate historical revenues; CDs peak around late 90s–2000.

Post-2000: shift towards digital — but total physical + digital revenues still decline from peak.

Inflation-adjusted values confirm real decline post-1999.
