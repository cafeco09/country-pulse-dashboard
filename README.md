# Country Pulse · Atlas of Happiness

**Country Pulse** is a map-first dashboard that visualises the “pulse” of countries using real happiness and life-evaluation data.

The dashboard shows how happy people report themselves to be across countries, using a large interactive world map where stronger red pulse effects represent higher happiness scores. Clicking a country reveals its score, global rank, trend, and the factors that help explain the final score.

## Live Demo

https://cafeco09.github.io/country-pulse-dashboard/

## What the Dashboard Shows

Country Pulse is structured around four layers:

1. **Global KPIs**
   - World average happiness score
   - Highest-ranked country
   - Number of countries improving
   - Gap between selected country and the leader
   - Selected country versus global average
   - Explained factor contribution where available

2. **Interactive World Map**
   - Grey world map for visual calm
   - Red heartbeat-style pulse markers
   - Larger pulse intensity for higher-scoring countries
   - Clickable countries
   - Search and filter controls

3. **Country Overview**
   - Selected country
   - Latest happiness score
   - Global rank
   - Trend over recent observations
   - Latest available year

4. **Factors Behind the Score**
   - GDP per capita
   - Social support
   - Healthy life expectancy
   - Freedom to make life choices
   - Generosity
   - Perceptions of corruption / trust
   - Residual or unexplained contribution

## Data Sources

The dashboard uses:

- **Our World in Data Cantril Ladder dataset** for country-level happiness / life-evaluation scores.
- **World Happiness Report factor data** where available for explanatory factor contributions.

The Cantril Ladder score represents how people evaluate their life on a scale from 0 to 10. The factor metrics are explanatory contributions used to understand what may be associated with higher or lower happiness scores. They should not be read as simple proof of direct causation.

## Design Direction

The dashboard is designed as an atmospheric “happiness atlas” rather than a traditional corporate analytics page.

Design choices include:

- Dark background for contrast
- Grey map to reduce visual noise
- Red heartbeat pulses to express emotional intensity
- Soft off-white text for readability
- Large centred map as the main visual focus
- KPIs above the map
- Country overview on the left
- Filters on the right
- Detailed metrics below the map

## Project Structure

```text
country-pulse-dashboard/
├── docs/
│   ├── index.html
│   └── data/
│       ├── happiness-cantril-ladder.csv
│       ├── whr_factors.csv
│       └── WHR26_Data_Figure_2.1.xlsx
└── README.md
