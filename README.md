# Climate Shock-Recovery Atlas for Global Agriculture 


```markdown
## Data collection

Sources
- FAOSTAT — country-level crop statistics (production, area, yield).[https://www.fao.org/faostat/en/#data/QCL]
- ECMWF (ERA5 / ERA5‑Land) — gridded climate predictors (temperature, precipitation, soil moisture, radiation), aggregated to monthly/seasonal.
- The variables from ECMWF are t2m, tcc, tp, ssr, si10. Here are the variable details below-
    TP — Total Precipitation

Amount of all precipitation (rain + snow + hail) accumulated over a time period.

Usually in meters or millimeters.

T2M — 2-Meter Temperature

Air temperature measured (or modeled) 2 meters above ground.

Same as standard “surface air temperature.”

TCC — Total Cloud Cover

Fraction of the sky covered by clouds.

Often given as 0–1 (0 = clear, 1 = fully cloudy) or in %.

SI10 — 10-Meter Wind Speed

Horizontal wind speed at 10 meters above ground.

Measured in m/s.

SSR — Surface Solar Radiation (Downwards)

Amount of shortwave (solar) radiation reaching the Earth’s surface.

Measured in J/m² or W/m².
Key processing (short)
- Harmonize country IDs and years; convert units.
- Aggregate ERA5 to countries (area‑weighted) and compute seasonal predictors(e.g., growing‑season mean temperature, cumulative precipitation).
- Run basic quality checks and minimal imputation; store cleaned tables for modelling.

Important
- Processed data, exact download queries, and preprocessing scripts are in /data and /scripts (provenance logged).
- Always cite FAOSTAT and ECMWF/ERA5 and follow their licensing/attribution.
```





