# Titanium, Materials Data Series #8

An interactive data dashboard and LinkedIn carousel on the metal with a split identity. Everyone pictures titanium as jets and hip implants, but over 95% of the titanium mined each year becomes white TiO2 pigment, not metal. The metal is real, but rare, and one country makes most of it.

Part of my Materials Data Series, where I take one material at a time and tell it as a materials engineer who works in data. Steel, aluminium, copper, rare earths, lithium, nickel and cobalt came first. Graphite is next.

**Live dashboard:** _(deploy `index.html` to Netlify/GitHub Pages)_

---

## What's inside

| File | What it is |
|------|-----------|
| `index.html` | Interactive Chart.js dashboard, 5 tabs: Production & Geography (with a highlighted world map), What 320,000 t Looks Like, Paint Not Planes, The China Factor, Why It Matters |
| `fetch_data.py` | Reproducible Python pipeline that compiles the cited figures into `data/*.csv` |
| `data/*.csv` | Tidy datasets (sponge production, mineral concentrates, pigment vs metal split, metal end uses, price, density, scale) |
| `carousel/index.html` | 9-slide LinkedIn carousel (1080x1080) |
| `Titanium_Materials_Carousel.pdf` | Exported carousel, ready to upload |
| `linkedin-post.txt` | Post caption, with the LinkedIn document title and GitHub slug at the top |

## Reproduce the data

```bash
python fetch_data.py      # writes data/*.csv
```

The dashboard embeds the same numbers in JS so it runs from `file://` with no server.

## What the data shows

- The world makes about **320,000 tonnes of titanium metal** (sponge) a year, roughly **10 kg every second**. That is tiny for a metal, near cobalt and lithium, even though titanium is the ninth most abundant element in the crust.
- **Over 95% of mined titanium becomes white TiO2 pigment**, the colour in paint, plastic, paper and sunscreen. For every tonne that becomes metal, about **17 tonnes becomes pigment**.
- The metal is mostly **aerospace** (about 48%), then industrial uses and **medical implants**. It is as strong as many steels at about **45% less weight**, corrosion-proof, and biocompatible.
- **China dominates the whole chain:** about **69% of titanium metal** (sponge), more than half of global TiO2 pigment capacity, and roughly a third of the ore. Japan and Russia are the other serious metal makers.
- The bottleneck is not the element, it is **making the metal**. The **Kroll process** is slow and energy-hungry, which keeps titanium metal scarce and expensive (about $13/kg in 2024, and rising rather than crashing).

## Sources

USGS Mineral Commodity Summaries 2025: the Titanium and Titanium Dioxide chapter (sponge production, prices, capacity) and the Titanium Mineral Concentrates chapter (ore production, reserves).

Output in kt and Mt; mineral concentrates in TiO2 content. Metal end-use shares are approximate 2024 estimates (the aerospace majority is per USGS). World sponge total excludes withheld US output. Figures rounded and attributed.

---

*Built by Ibtisam Ahmed Khan · June 2026 · [linkedin.com/in/ibtisam-ahmed-khan](https://linkedin.com/in/ibtisam-ahmed-khan)*
