# Level 5 — Graph Thinking

**Type:** Written + 1 diagram  
**Deadline:** Wednesday May 13, 2026 23:59 UTC  
**Submission:** PR to `lpi-developer-kit` → `submissions/<your-github-username>/level5/answers.md`  
**PR title:** `level-5: Your Name`  
**Time:** 2-3 hours  

---

## Context

You've been given a **real factory production dataset** (`challenges/data/`). It comes from a Swedish steel fabrication company running 8 construction projects across 7 production stations. The data is in 3 CSV files:

- `factory_production.csv` — 60 rows: projects × products × stations × weeks (hours planned vs actual)
- `factory_workers.csv` — 14 workers with stations, certifications, roles
- `factory_capacity.csv` — 8 weeks of capacity vs demand

This is actual production planning data. The company currently manages it in a 46-sheet Excel workbook. Your job over L5+L6 is to turn it into something better.

---

## 5 Questions (20 pts each)

### Q1. Model It (20 pts)

Look at the 3 CSVs. Design a **graph schema** that captures the relationships between projects, products, stations, workers, and weeks.

- Draw a diagram with node labels and relationship types (hand-drawn photo, draw.io, ASCII — any format)
- At least **6 node labels** and **8 relationship types**
- At least 2 relationships must carry data (e.g., `WORKED_AT {hours: 38.5, week: "w1"}`)
- Save as `schema.png`

### Q2. Why Not Just SQL? (20 pts)

Write ONE query that answers: *"Which workers are certified to cover Station 016 (Gjutning) when Per Gustafsson is on vacation, and which projects would be affected?"*

1. Write it in SQL (assume reasonable tables)
2. Write it in Cypher (using your schema from Q1)
3. In 2-3 sentences: what does the graph version make obvious that SQL hides?

### Q3. Spot the Bottleneck (20 pts)

Look at `factory_capacity.csv`. Weeks w4 and w7 show capacity deficits (-45 and -60 hours).

1. Using `factory_production.csv`, identify which projects/stations are causing the overload
2. Write a Cypher query that would find: *"All projects where actual_hours > planned_hours by more than 10%, grouped by station"*
3. How would you model this alert as a graph pattern? (e.g., a `(:Bottleneck)` node, a relationship property, or something else?)

### Q4. Vector Search Use Case (20 pts)

The factory gets new project requests described in free text, like:
> "450 meters of IQB beams for a hospital extension in Linköping, similar scope to previous hospital projects, tight timeline"

1. What would you embed? (project descriptions? product specs? something else?)
2. Write a query that combines: "find similar past projects [vector] that used the same stations and had variance < 5% [graph]"
3. Why is this more useful than just filtering by product type?

### Q5. Your L6 Plan (20 pts)

Write your blueprint for Level 6. Be specific:
1. Your node labels and what CSV columns map to them
2. Your relationship types and what creates them
3. 3 Streamlit dashboard panels you'll build (e.g., "project timeline heatmap", "station load bar chart", "worker coverage matrix")
4. Which `/query/{id}` endpoints you'll implement

---

## Submission

```
submissions/<your-github-username>/level5/
├── answers.md
└── schema.png
```
