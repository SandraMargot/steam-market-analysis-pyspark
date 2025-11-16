# Steam Marketplace Insights
A data-driven overview of the global PC gaming ecosystem on Steam.

---

## What it does
- Analyzes the Steam catalogue to understand today’s gaming landscape  
- Identifies key trends in publishers, genres, platforms, pricing, and ratings  
- Highlights what drives game popularity and player engagement  
- Provides actionable insights for strategic game development and positioning

---

## Data Used
### Source
Steam dataset (nested JSON) from S3  
`steam_game_output.json`

### Core fields explored
- Publisher & developer metadata  
- Genres & categories  
- Release dates  
- Price & discount information  
- Positive/negative review counts  
- Supported platforms  
- Languages and age ratings

---

## Analysis Focus
### Market Overview
- Most active publishers  
- Highest-rated titles  
- Release patterns over time (including the Covid period)  
- Pricing and discount distribution  

### Genres
- Most represented genres  
- Genres with the best review ratios  
- Genre–publisher affinities  
- High-value genres (based on pricing signals)

### Platforms
- Availability across Windows, Mac, and Linux  
- Genre–platform preferences

---

## Tech Stack
- Databricks (Free Edition)  
- PySpark (handling nested and semi-structured JSON)  
- Transformations using `explode()`, `getField()`, and date parsing  
- Visualizations built with Databricks notebook dashboard (exported with outputs) as "publish" is not available

---

## 📁 Key Files
- `Project_Steam_Sandra.ipynb` — Data preparation & EDA  
- `Project_Steam_Sandra-visuals.ipynb` — All charts (exported with outputs)

---

## Notes
Databricks no longer supports public notebook publishing.  
All visualizations are therefore included directly in the exported notebooks stored in this repository.
