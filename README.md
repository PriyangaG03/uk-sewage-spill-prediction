# UK Sewage Spill Early-Warning System

Predicting storm overflow sewage spills in the North West of England 24–48 hours ahead, using rainfall, river level and historical spill data.

## Problem
In many UK towns, rainwater and household sewage share the same pipes. During heavy rain these pipes overflow, and untreated sewage is released into rivers and the sea through storm overflows. Spill data is published, but only after the event, so swimmers, anglers and local communities find out too late.

## Goal
- Predict the probability that each storm overflow will spill in the next 24–48 hours
- Estimate how long a spill is likely to last
- Show daily risk (low / medium / high) on a live map

## Success metric
Catch most real spills a day in advance (high recall) while keeping false alarms reasonable, and beat a simple rainfall-threshold rule.

## Data sources
- **Spill events:** [Environment Agency – Event Duration Monitoring, Storm Overflow Start/Stop Detailed Data](https://environment.data.gov.uk/dataset/e9677ac1-fd32-4ceb-88a0-2735be5f27c7)
- **Rainfall:** [Open-Meteo Historical Weather API](https://open-meteo.com/)

## Status
🚧 In progress: Day 2 complete (data collection)
- ✅ Project setup and structure
- ✅ Rainfall data: Manchester daily rainfall 2020–2026 (Open-Meteo API)
- ✅ Spill data: 465,371 United Utilities storm overflow events, 2024 – Sep 2026
- ⏳ Next: match outlets to locations and rainfall