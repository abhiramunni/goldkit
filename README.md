# GoldKit — Buy Gold Smart

Gold is down almost 15% in a month and at a 14-month low (22 Nov 2026). GoldKit helps you buy gold like someone who knows the price: today's rate, the real cost of a necklace once making charges and GST are added, what the gold you already own is worth, and the hallmark checks to run before you pay.

**Live:** https://abhiramunni.github.io/goldkit/

## What it does

- **Today's gold rate** — 24K ₹12,127/g, 22K ₹11,108/g, 18K ₹9,095/g (indicative, 22 Nov 2026), with MCX futures, world price, rupee rate and silver.
- **30-day trend chart** — 24K per 10 g across 10 published daily rates (22 Oct – 22 Nov 2026), with the 30-day low, high and −14.8% change.
- **"Should I buy now?"** — plain-words read on the fall (hawkish US Fed, strong dollar, high Treasury yields) with an honest "nobody can time the bottom" line. Context, not investment advice.
- **Jewellery bill calculator** — weight + purity + making % + wastage % → an itemised bill: metal value, wastage, making, GST (3% on metal, 5% on making) and the all-in total. Default 8 g, 22K, 12% making, 2% wastage = ₹1,04,557.
- **Compare jewellers** — save quotes from different shops for the same piece; the cheapest is highlighted. Seeded with two sample quotes (Tanishq ₹1,10,156 vs Malabar Gold ₹1,02,690 for the same 8 g 22K piece).
- **My gold stash** — log what you own (grams, purity, price paid) and see its value today vs what you paid. Seeded with three samples: worth ₹3,63,608 against ₹2,47,200 paid (+47.1%).
- **Hallmark & HUID** — purity table (24K 999 / 22K 916 / 18K 750 / 14K 583) and how to verify the 6-digit HUID on the BIS Care app.
- **Investing in gold** — SGB vs gold ETF vs coins & bars vs digital gold vs jewellery, in one honest table.
- **8-point buying checklist** — with a progress ring, for the counter.
- **6 plain-language guides** — making charges, hallmark & HUID, 22K vs 24K, selling old gold, SGB vs ETF, wedding gold budgets.

## How it works

- One `index.html` (plus the two photo files below) — no backend, no signup. Everything is saved in your browser (localStorage) only.
- The published site on GitHub Pages is `index.html` plus the two photo files (`goldkit-hero.webp`, `goldkit-flatlay.webp`) in the repo root; the page loads both photos by filename.
- Cinematic gold-coin intro (tap to skip, quick on return visits) and a 3-step tour on first visit.

## Rates & sources

Rates are indicative for 22 Nov 2026, from published market rates: 24K ₹1,21,271 / 10 g, 22K ₹1,11,084 / 10 g, 18K ₹90,953 / 10 g, MCX gold futures ₹1,21,949 / 10 g, silver ₹1,49,590 / kg, world gold $3,539/oz at ₹92.68/$. The 30-day series uses the published daily 24K rates from 22 Oct to 22 Nov 2026. Jeweller prices, making charges and wastage vary by shop and design.

## Tech

- Single HTML file, vanilla JS, canvas chart, Fraunces + Inter.
- QA: headless jsdom assertions (`qa-test.js`), `node --check` clean, zero uncaught JS errors.
