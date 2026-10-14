# HCDE410
Files for HCDE410 - Assignment A1

Adapted from # cdsw-2020 https://wiki.communitydata.science/Seattle_open_data

# A1 — Working with Open Data

**Dataset:** Burke Gilman Trail north of NE 70th St Bicycle Counter (hourly bike and pedestrian counts, by direction of travel)

**Source:** https://data.seattle.gov/Transportation/Burke-Gilman-Trail-north-of-NE-70th-St-Bicycle-Counter/2z5v-ecg8 (pulled 2026-10-13)

**Publisher:** City of Seattle, Seattle Department of Transportation (SDOT)

**License / terms of use:** Public Domain, as listed on the dataset's data.seattle.gov page. I still credit the City of Seattle as the source. The code in this folder is under the MIT License (see `LICENSE`).

## Questions I asked
- **Q1:** When is the trail busiest and quietest? (Bikes and pedestrians combined, by single hour. Busiest: hour 17; quietest: hour 2.)
- **Q2:** Do cyclists and pedestrians use the trail at different times of day? (Hourly totals for each mode.)
- **Q3:** Is there evidence of commuting versus recreation? (Totals by day of week, and cyclists by hour on weekdays vs. weekends.)
- **Q4:** Direction and flow. Are mornings mostly one direction and evenings the other? (Weekday cyclists by hour, northbound vs. southbound.)

## How to re-run
Open `A1.ipynb` and run all cells (needs `requests`, `pandas`, `matplotlib`). The notebook pulls the data from the Seattle open-data portal, so it needs an internet connection, and the data is refreshed monthly, so numbers may shift slightly if the data is pulled again later.

## Limitation / bias in the data
The counter records only one spot on the trail (north of NE 70th St), so it can't tell us where people start or finish their trips, and the patterns here may not hold for other parts of the trail. It also counts passes, not people, so one person riding past twice is counted twice, and it can't tell commuters from recreational users. I inferred commuting from timing and direction, which is suggestive but not proof.

## AI use
I used an AI assistant for help with coding and creating the graphs, then interpreted them and further used AI for wording and checking my interpretations made sense.