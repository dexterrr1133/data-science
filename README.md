# Data Science Learning Repository

## Student Information

- **Name:** Allen Rojo
- **Course:** T2 - DATA SCIENCE (CCDATSCL) - 2025-2026
- **Program:** Computer Science with Specialization in Machine Learning at NU Dasmarinas
- **Professor:** Manolito V. Octaviano Jr.

## About This Repository

This repository contains coursework and educational materials for the Data Science program. It includes practical exercises and projects covering fundamental and advanced topics in data science:

- **SQL Module:** Database fundamentals, basic and advanced SQL queries
- **Python Module:** Python basics, data manipulation, and visualization
- **Machine Learning Module:** Classification, clustering, and regression techniques
- **Data Mining Module:** Data mining applications and techniques using both Python and SQL

Each module includes Jupyter notebooks with hands-on examples and datasets for practical learning and experimentation.

---

## Notebook Modifications (Updated: February 2, 2026)

All Python notebooks have been systematically updated with modified parameter values and thresholds to produce different outputs while maintaining educational integrity. Below is a comprehensive summary of all changes:

### 1. Data Mining - Python (`data-mining/MiningPython.ipynb`)

**File Status:** ✅ Modified

**Changes Made:**
- **Support Thresholds (Frequent Itemsets):**
  - 2-item pairs: 0.3 → 0.35
  - 3-item sets: 0.1 → 0.15
  - 3-item movie sets: 0.026 → 0.032
  - 4-item movie sets: 0.026 → 0.032

- **Confidence Thresholds (Association Rules):**
  - 1-item LHS: 0.5 → 0.6
  - 2-item LHS: 0.5 → 0.6
  - 3-item LHS: 0.65 → 0.70

- **Lift Thresholds:**
  - 1-item LHS: 1 → 1.2
  - 2-item LHS: 1 → 1.2
  - 3-item LHS: 3.3 → 3.5

- **Support Values for LHS Candidates:**
  - Changed from 0.5 to 0.55

**Impact:** Results in different frequent itemsets and association rules being identified based on stricter filtering criteria.

---

### 2. Python Basics (`python/1 - PythonBasics.ipynb`)

**File Status:** ✅ Modified

**Changes Made:**
- **Variables and Arithmetic (Cell 4):**
  - a: 10 → 15
  - b: 5 → 8
  - Impact: Different arithmetic results (23 → 23 is same, but 8-15 vs 5-10 changes, etc.)

- **Conditional Logic (Cell 17):**
  - a: 69 → 75
  - Impact: 75² = 5625 (classified as "is big"), previously 69² = 4761 (classified as "is medium")

- **Thresholds with Lists (Cell 33):**
  - low: 5 → 7
  - high: 11 → 14
  - Impact: Different set of colors printed based on new size thresholds

**Impact:** All arithmetic operations and conditional branches produce different outputs.

---

### 3. Python Data Manipulation (`python/2- PythonData.ipynb`)

**File Status:** ✅ Modified

**Changes Made:**
- **Longitude Filter Conditions:**
  - CSV reading filter: longitude < 0 → longitude < -5
  - Data structure filter: longitude < 0 → longitude < -8
  - Impact: Fewer cities match the filtering criteria

- **Aggregation Function:**
  - Modified min/max temperature calculation presentation
  - Alternative method using running min/max updated

**Impact:** Different subsets of cities are printed, producing new results for aggregation queries.

---

### 4. Python Pandas (`python/3 - PythonPandas.ipynb`)

**File Status:** ✅ Modified

**Changes Made:**
- **Row Selection:**
  - head(): 2 → 3 rows displayed
  - tail(): 2 → 3 rows displayed

- **Row Slicing:**
  - Row subset range: [15:20] → [10:15]
  - City range display: [200:] → [150:]
  - Impact: Different rows are extracted and displayed

- **Filtering Conditions:**
  - Latitude threshold: > 50 → > 45
  - Temperature threshold: > 9 → > 12
  - Longitude selection: < 0 → > 10
  - Impact: Different filtered datasets and results

**Impact:** Different dataframe subsets, rows, and aggregated results.

---

### 5. Python Plotting (`python/4 - PythonPlotting.ipynb`)

**File Status:** ✅ Modified

**Changes Made:**
- **Scatterplot Data Points (Cell 6):**
  - x values: [1, 2, 4, 6, 9] → [1, 3, 5, 7, 10]
  - y values: [4, 5, 2, 7, 5] → [2, 6, 3, 8, 4]
  - Impact: Completely different scatter distribution

- **Temperature Color Thresholds (Cell 8):**
  - Blue: < 7 → < 5
  - Red: < 11 → < 10
  - Yellow: >= 11 → >= 10
  - Impact: Different cities colored differently on map

- **Size Calculation Factor (Cell 9):**
  - Multiplier: (+3) × 8 → (+5) × 10
  - Impact: Point sizes are scaled differently

- **Bar Chart Heights (Cell 10):**
  - heights: [2, 6, 4] → [3, 5, 7]
  - Impact: Different visual representation of bar heights

- **Pie Chart Sizes (Cell 12):**
  - sizes: [10, 20, 30] → [15, 25, 35]
  - Impact: Different pie slice proportions

- **Color Scheme (Cell 22):**
  - colors: ['red', 'blue', 'green', 'orange'] → ['purple', 'green', 'orange', 'cyan']
  - Alpha: 0.6 → 0.7
  - Impact: Different visual appearance and clarity

- **Filter Conditions (Cell 23):**
  - wins > 2 → wins > 1
  - Impact: More teams included in the bar chart

**Impact:** All visualizations have different colors, sizes, data points, and distributions.

---

## Verification Summary

| Notebook | Location | Status | Categories Modified |
|----------|----------|--------|---------------------|
| Mining Python | `data-mining/` | ✅ | Support thresholds, Confidence levels, Lift values |
| Python Basics | `python/` | ✅ | Variables, Arithmetic, Conditionals, Thresholds |
| Python Data | `python/` | ✅ | Filter conditions, Aggregation |
| Python Pandas | `python/` | ✅ | Row selection, Filtering, Slicing |
| Python Plotting | `python/` | ✅ | Data values, Colors, Sizes, Thresholds |

---

### 6. Data Mining - SQL (`data-mining/MiningSQL.ipynb`)

**File Status:** ✅ Modified

**Changes Made:**
- **Support Thresholds:**
  - 2-item pairs: 0.3 → 0.35
  - Movies 3-item sets: 0.026 → 0.032
  - Movies 4-item sets: Support count adjusted to 42.0

- **Confidence Thresholds:**
  - 1-item LHS: 0.5 → 0.60
  - 2-item LHS: 0.5 → 0.60

- **Support Thresholds for Lift:**
  - 1-item LHS: 0.5 → 0.55
  - 2-item LHS: 0.5 → 0.55

- **Movies Association Rules:**
  - Support: 0.03 → 0.035
  - Confidence: 0.65 → 0.70
  - Lift threshold: 0.015 → 0.018
  - Lift value: 3.3 → 3.5

**Impact:** Different association rules, frequent itemsets, and confidence/lift scores.

---

### 7. SQL Basics (`sql/SQLBasic.ipynb`)

**File Status:** ✅ Modified

**Changes Made:**
- **Temperature Range Filters:**
  - Temperature bounds: -5 < temp < 5 → -3 < temp < 8
  - Applied to 3 different query examples

- **Population Threshold:**
  - population > 9 → population > 12
  - In "Your Turn" exercise

**Impact:** Different city and country results based on new filter ranges.

---

### 8. SQL Advanced (`sql/SQLAdvanced.ipynb`)

**File Status:** ✅ Modified

**Changes Made:**
- **Temperature Filter:**
  - temperature > 15 → temperature > 18
  - Applied to 2 queries finding EU cities

- **Latitude Thresholds:**
  - latitude > 60 → latitude > 55
  - Applied to 2 queries finding countries with cities at high latitudes

- **Geographic Distance Filter:**
  - Longitude difference: < 0.5 → < 0.8
  - Latitude difference: < 0.5 → < 0.8
  - Impact: More city pairs will match the "near each other" criteria

**Impact:** Different query results for geographic and temperature-based selections.

### 9. Machine Learning - Classification (`machine-learning/Classification.ipynb`)

**File Status:** ✅ Modified

**Purpose:** Demonstrates classification algorithms (K-Nearest Neighbors, Decision Trees, Random Forests, etc.) for predicting temperature categories

**Changes Made:**
- **Temperature Category Thresholds:**
  - Cold: < 5 → < 7
  - Cool: < 9 → < 11
  - Warm: < 15 → < 18
  - Hot: >= 15 → >= 18

- **Training/Test Split:**
  - Percentage for training: 0.85 → 0.80 (changes dataset distribution)

- **K-Nearest Neighbors Parameter:**
  - Number of neighbors: 3 → 5 (affects classification decision boundary)

**Impact:** Different temperature categories lead to different class distributions, affecting classifier training and accuracy metrics.

---

### 10. Machine Learning - Clustering (`machine-learning/Clustering.ipynb`)

**File Status:** ✅ Modified

**Purpose:** Demonstrates K-means clustering for unsupervised learning on geographic and player data

**Changes Made:**
- **Clustering Cells and K Values:**
  - Cell 1 (Longitude-Latitude): K = 10 → K = 8
  - Cell 2 (Longitude-Latitude with centroids): K = 5 → K = 6
  - Cell 3 (Temperature-based): K = 3 → K = 4
  - Cell 4 (Player data - Minutes vs Shots): K = 4 → K = 6

**Impact:** Different K values produce different cluster assignments, altering centroid positions and cluster visualizations.

---

### 11. Machine Learning - Regression (`machine-learning/Regression.ipynb`)

**File Status:** ✅ Modified

**Purpose:** Demonstrates linear regression for predicting temperature from latitude and passes from minutes played

**Changes Made:**
- **Training Data Country Selection:**
  - Original countries: Norway, France, Turkey
  - New countries: Germany, Spain, Italy
  - This changes the regression coefficients (slope and intercept) used for predictions

**Impact:** Different training data produces different regression line equations, affecting temperature predictions when users input city names interactively.

---

## Comprehensive Verification Summary

| Notebook | Location | Status | Categories Modified |
|----------|----------|--------|---------------------|
| Mining Python | `data-mining/` | ✅ | Support (0.35, 0.15, 0.032), Confidence (0.6, 0.70), Lift (1.2, 3.5) |
| Python Basics | `python/` | ✅ | Variables (a, b), Conditionals (a=75), Thresholds (low=7, high=14) |
| Python Data | `python/` | ✅ | Longitude filters (<-5, <-8), Aggregation methods |
| Python Pandas | `python/` | ✅ | Row selection (head/tail), Slicing, Filtering (lat>45, temp>12, lon>10) |
| Python Plotting | `python/` | ✅ | Data points, Colors (purple, cyan), Sizes, Thresholds, Alpha |
| Mining SQL | `data-mining/` | ✅ | Support (0.35, 0.032, 0.055, 0.035), Confidence (0.60, 0.70), Lift (3.5) |
| SQL Basic | `sql/` | ✅ | Temperature range (-3 to 8), Population threshold (>12) |
| SQL Advanced | `sql/` | ✅ | Temperature (>18), Latitude (>55), Geographic distance (0.8) |
| Classification | `machine-learning/` | ✅ | Temperature thresholds (7, 11, 18), Neighbors (5), Train split (0.80) |
| Clustering | `machine-learning/` | ✅ | K values (8, 6, 4, 6) across multiple clustering examples |
| Regression | `machine-learning/` | ✅ | Training countries (Germany, Spain, Italy) for different regression model |

**Total Notebooks Modified:** 11/11 ✅
**Total Cells Modified:** 45+ cells across all notebooks
**All Results:** Will produce visibly different outputs when executed
