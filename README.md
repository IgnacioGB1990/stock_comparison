

https://github.com/user-attachments/assets/d8910b13-b3fb-4217-a575-e7c09393999f

# Dow Jones Stock Performance Dashboard

An interactive stock analysis tool built entirely in **Microsoft Excel**, using native **dynamic arrays and spilled ranges** — no VBA, no macros, no add-ins. Users pick any stock (or pair of stocks) from the Dow Jones Industrial Average and instantly see filtered performance data pulled live from a 5-year historical dataset.

## Overview

The workbook has two main views:

| View | Description |
|---|---|
| **Stock Analysis** | Deep-dive into a single Dow Jones stock (`[Stock A]`) — performance data filters dynamically based on the selected ticker and time range. |
| **Stock Comparison** | Side-by-side comparison of two stocks (`[Stock A] vs [Stock B]`) — both series filter and spill independently from the same underlying dataset. |

In both views, users can select any point within the last 5 years as a starting date, and the output automatically recalculates and resizes to match.

## Features

### 1. Stock Analysis
- Select any Dow Jones constituent from a dropdown (data validation list).
- Choose a starting point anywhere within the trailing 5 years.
- Performance data (price history, returns, etc.) filters live from the master dataset and **spills** into the sheet — the output range grows or shrinks automatically as the selection changes, with no helper columns or manually dragged formulas.

### 2. Stock Comparison
- Two independent stock selectors (`Stock A` and `Stock B`) driving two spilled ranges side by side.
- Both series respond to the same dynamic date filter, making it easy to visually and numerically compare performance over identical windows.
- Charts are bound directly to the spill ranges, so they resize and update automatically as the filtered data changes — no manual chart range edits needed.



```markdown
# Project Overview

This repository is organized into three main folders:



├── dashboard/
├── data/
└──scripts/

```

## Folder Structure

### 📊 dashboard/

Contains stock comparison dashboard in Excel.

---

### 📁 data/

Stores all raw data generated from Python script stored in csv.

---

### 🐍 scripts/

Contains Python script.

---

## Project Workflow

1. Collect or generate data using the scripts in `scripts/`.
2. Store raw or processed datasets in `data/`.
3. Build reports and visualizations using the files in `dashboard/`.

This structure helps keep the project organized, reproducible, and easy to navigate.

