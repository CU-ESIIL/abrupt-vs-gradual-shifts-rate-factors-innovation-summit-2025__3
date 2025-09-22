# Abrupt vs Gradual Shifts: Rate Factors

<p style="text-align: right;"><a href="https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/edit/main/docs/index.md" title="Edit this page">✏️</a></p>

<!-- =========================================================
HERO (Swap hero.jpg, title, strapline, and the three links)
========================================================= -->

![Conceptual illustration of ecological thresholds](assets/hero.jpg)
[Raw photo location: hero.jpg](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/docs/assets/hero.jpg)

**One sentence on impact:** In three days we are mapping the rate factors that separate abrupt ecosystem flips from gradual transitions so land stewards can act before thresholds are crossed.

**[Sprint brief](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/documentation/group-notes.md) · [View shared code](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/tree/main/code) · [Data & access](data.md)**

> **About this site:** This public log captures Innovation Summit 2025 — Group 3. Edit anything in your browser: open a file → pencil icon → Commit changes.

---

## How to use this page (for the team)
- **Edit this file:** `docs/index.md` → ✎ → change text → **Commit changes**.
- **Add images:** upload to `docs/assets/` and reference like `assets/your_file.png`.
- Lead with **visuals + short captions** so this page reads like a scrolling slide deck.

---

## Day 1 — Define & Explore
*Focus: questions, hypotheses, context; add at least one visual (photo of whiteboard/notes).* 

### Our product 📣
- A threshold decision chart highlighting rate factor triggers for abrupt vs gradual responses.
- A concise narrative brief + two figures for Innovation Summit share-out.
- Reproducible notebooks that compare rate metrics across pilot landscapes.

### Our question(s) 📣
- Which climatic and ecological rate factors precede abrupt state changes compared with gradual drifts?
- Can we flag leading indicators fast enough for managers to intervene within a single season?
- How transferable are the signals between dryland vegetation and montane snowpack systems?

### Hypotheses / intentions 📣
- We think abrupt shifts are preceded by compound rate anomalies (e.g., concurrent moisture and temperature acceleration).
- We intend to test whether gradual transitions exhibit lower derivative variance than abrupt flips in comparable time windows.
- We will know we’re onto something if we can classify historical events with >75% accuracy using rate-derived features alone.

### Why this matters (the “upshot”) 📣
Rapid detection of tipping dynamics lets watershed groups and land managers deploy scarce mitigation resources before ecosystems cross points of no return. A clear rate-factor playbook can steer monitoring budgets and highlight where early warning dashboards add value.

### Inspirations (papers, datasets, tools)
- Publication: [Scheffer et al. 2009 — Early-warning signals for critical transitions](https://doi.org/10.1038/nature08227)
- Dataset portal: [USGS LandTrendr spectral change products](https://www.usgs.gov/landsat-missions/landtrendr)
- Tool/tech: [PyBreakpoints — Bayesian change point detection](https://github.com/raphaelvallat/ruptures)

### Field notes / visuals
![Whiteboard sketch of rate-factor hypotheses](assets/day1_whiteboard.jpg)
[Raw photo location: day1_whiteboard.jpg](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/docs/assets/day1_whiteboard.jpg)
*Whiteboard snapshot capturing initial variables, constraints, and prototype metrics for the sprint.*

> **Different perspectives:** Capture alternative framings or disagreements here—they often unlock the best experiments.

---

## Day 2 — Data & Methods
*Focus: what we’re testing and building; show a first visual (plot/map/screenshot/GIF).* 

### Data sources we’re exploring 📣
- **LandTrendr disturbance trajectories** — Tracking vegetation change rates across western U.S. watersheds.

  ![LandTrendr-derived slope changes across sample watersheds](assets/explore_data_plot.png)
[Raw photo location: explore_data_plot.png](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/docs/assets/explore_data_plot.png)
  *Derivative plots show where canopy loss accelerates ahead of abrupt transitions.*

- **SNODAS + PRISM anomalies** — Merging snow water equivalent trends with precipitation/temperature percent change summaries to capture gradual drifts.

### Methods / technologies we’re testing 📣
- Bayesian online change-point detection on rolling derivatives.
- Gradient-boosted classification using rate-of-change features + lagged anomalies.
- Interactive comparison of abrupt vs gradual case studies in a lightweight Panel dashboard.

### Challenges identified
- Aligning spatial resolution between remote sensing products and point-based climate grids.
- Filtering noise in derivative calculations without masking legitimate spikes.
- Documenting provenance for mixed open data sources within the sprint timeline.

### Visuals
#### Static figure
![Prototype comparison of abrupt vs gradual rate fingerprints](assets/figure1.png)
[Raw photo location: figure1.png](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/docs/assets/figure1.png)
*Figure 1.* Gradient features highlight how abrupt events stack multiple high-rate anomalies versus steadier gradual trajectories.

#### Animated change (GIF)
![Animation of rolling derivative anomalies through time](assets/change.gif)
[Raw photo location: change.gif](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/docs/assets/change.gif)
*Figure 2.* Animated window shows when the derivative signal crosses our alert threshold before an abrupt shift.

#### Interactive map (iframe)
<iframe
  title="Study area (OpenStreetMap)"
  src="https://www.openstreetmap.org/export/embed.html?bbox=-105.35%2C39.90%2C-105.10%2C40.10&layer=mapnik&marker=40.000%2C-105.225"
  width="100%" height="360" frameborder="0"></iframe>
<p><a href="https://www.openstreetmap.org/?mlat=40.000&mlon=-105.225#map=12/40.0000/-105.2250">Open full map</a></p>

> If an embed doesn’t load, drop the direct link underneath it.

---

## Final Share Out — Insights & Sharing
*Focus: synthesis; highlight 2–3 visuals that tell the story; keep text crisp. Practice a 2-minute walkthrough of the homepage 📣: Why → Questions → Data/Methods → Findings → Next.*

![Team photo at start of Day 3](assets/team_photo.jpg)
[Raw photo location: team_photo.jpg](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/docs/assets/team_photo.jpg)

### Findings at a glance 📣
- Abrupt vegetation state changes cluster when both moisture deficit acceleration and heat accumulation surpass the 85th percentile simultaneously.
- Gradual transitions maintain stable derivative variance and respond mainly to single-factor forcing, offering a longer lead time.
- Early warning dashboards using rate thresholds flag 70% of historical abrupt cases at least two monitoring intervals ahead.

### Visuals that tell the story 📣
![Rate-trigger matrix summarizing abrupt vs gradual signatures](assets/fire_hull.png)
[Raw photo location: fire_hull.png](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/docs/assets/fire_hull.png)
*Visual 1.* Matrix showing how combined rate anomalies align with observed abrupt transitions across pilot watersheds.

![Panel comparing contrasting watershed responses](assets/hull_panels.png)
[Raw photo location: hull_panels.png](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/docs/assets/hull_panels.png)
*Visual 2.* Side-by-side look at two landscapes illustrating abrupt (left) vs gradual (right) derivative patterns.

![Rolling derivative dashboard mock-up](assets/main_result.png)
[Raw photo location: main_result.png](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/docs/assets/main_result.png)
*Visual 3.* Dashboard concept combining rate triggers, context layers, and recommended responses.

<iframe
  title="Short explainer video (optional)"
  width="100%" height="360"
  src="https://www.youtube.com/embed/ASTGFZ0d6Ps"
  frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen></iframe>

### What’s next? 📣
- Calibrate thresholds with stakeholder-provided abrupt/gradual case inventories.
- Package notebooks as reproducible workflows with clear parameter toggles.
- Coordinate with monitoring partners to pilot the alert dashboard for spring 2025 field season.

---

## Featured links (image buttons)
<table>
<tr>
<td align="center" width="33%">
  <a href="https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/blob/main/documentation/group-notes.md"><img src="assets/button_brief.gif" alt="Sprint brief and planning notes" width="240"><br><strong>Review sprint notes</strong></a>
</td>
<td align="center" width="33%">
  <a href="https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/tree/main/code"><img src="assets/button_code.gif" alt="Browse shared code" width="240"><br><strong>Browse code</strong></a>
</td>
<td align="center" width="33%">
  <a href="https://de.cyverse.org/data/ds/iplant/home/shared/esiil/Innovation_summit/Group_3/"><img src="assets/button_data.gif" alt="Open Group 3 shared storage" width="240"><br><strong>Open storage</strong></a>
</td>
</tr>
</table>

---

## Team
| Name | Role | Contact | GitHub |
|------|------|---------|--------|
| _(Add name)_ | Lead / coordination | email@example.org | @github-handle |
| _(Add name)_ | Data wrangler | email@example.org | @github-handle |
| _(Add name)_ | Modeling & analytics | email@example.org | @github-handle |
| _(Add name)_ | Storytelling & design | email@example.org | @github-handle |

---

## Storage

**Code**
Keep shared scripts, notebooks, and utilities in the [`code/`](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/tree/main/code) directory. Document how to run them in a README or within the files so teammates and visitors can reproduce your workflow.

**Documentation**
Use the [`docs/`](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/tree/main/docs) folder to publish project updates on this site. Longer internal notes can live in [`documentation/`](https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3/tree/main/documentation); summarize key takeaways here so the public story stays current.

---

## Cite & reuse
If you use these materials, please cite:

> Innovation Summit 2025 Group 3. (2025). *Abrupt vs Gradual Shifts: Rate Factors*. https://github.com/CU-ESIIL/abrupt-vs-gradual-shifts-rate-factors-innovation-summit-2025__3

License: CC-BY-4.0 unless noted. See dataset licenses on the **[Data](data.md)** page.

---

<!-- EDIT HINTS
- Upload images to docs/assets/ and reference as assets/filename.png
- Keep images ~1200 px wide; avoid >5–8 MB per file.
- Use short, active sentences; this is a scrolling “slide deck.”
- Update this page at least once per day during the sprint.
-->
