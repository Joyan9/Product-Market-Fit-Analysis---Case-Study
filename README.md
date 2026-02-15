# Product-Market-Fit Analysis: AirPure Air Purifier

## 📋 Project Overview

This project is a **product-market-fit analysis for AirPure**, a year-round air purifier system designed for India's pollution patterns. The analysis leverages multiple data sources to identify optimal market entry points, validate product requirements, and establish a data-driven go-to-market strategy.

**Objective:** Determine the most promising launch cities, validate core product features, and quantify market opportunity through pollution seasonality analysis.

---

## 🎯 Key Findings & Outcomes

### **Market Opportunity**
- **18 high-risk cities** identified across India with ≥40% "bad air days"
- **NCR metro region** offers the largest addressable market:
  - **Delhi**: 22M population, 51% bad days (worst AQI: 401)
  - **Ghaziabad**: 3.1M population, 49% bad days
  - **Faridabad**: 2.1M population, 45% bad days

### **Pollution Seasonality (High-Risk Cities)**
| Season | % Bad Days | Avg AQI | Status |
|--------|-----------|---------|--------|
| **Winter** | 81% | 284 | 4 out of 5 days hazardous |
| **Summer** | 41% | 189 | 2 out of 5 days bad |
| **Monsoon** | 22% | 139 | 1 out of 5 days bad |

**Insight:** AirPure is **not a seasonal product**—41% summer pollution and 22% monsoon pollution validate year-round demand beyond winter.

### **Primary Pollutant: PM2.5**
- **PM2.5 present in 73% of bad air days** (highest frequency among all pollutants)
- Frequently occurs with PM10, O3, and CO in dangerous combinations
- Justifies true HEPA H13 filter + activated carbon layer as core product requirements

### **Competitive Positioning**
AirPure Premium (₹18-22K) uniquely combines:
- **HEPA + Carbon filtration** (matches only premium competitors)
- **PM2.5 sensor with auto mode** (matches Dyson TP10, exceeds Coway/Philips)
- **Smart app control + seasonal presets** (WiFi connectivity differentiator)
- **350+ m³/h CADR** (matches market leaders at mid-premium price point)

---

## 📊 Analysis Methodology

### **Data Sources**
1. **Air Quality Data** - Day-wise AQI, pollutant types, and status for 290+ Indian cities (2020-2024)
2. **Population Projections** - State-level demographic forecasts (2011-2025) from official government data
3. **Vehicle Registration Data** - Pollution contributor analysis across India
4. **Disease Surveillance Data** - Health impact correlation with air quality patterns
5. **Market Benchmark Data** - Competitor feature matrix and pricing analysis

### **Analysis Approach**
- **Exploratory Data Analysis (EDA):** Pollution trend identification, seasonality patterns, and pollutant frequency analysis
- **City Risk Scoring:** Multi-factor ranking combining AQI severity, bad days percentage, and population size
- **Population Scaling:** State growth multipliers applied to 2011 census data to estimate 2025 market size
- **Competitive Benchmarking:** Feature-to-price positioning against 5 major market competitors

---

## 🚀 Launch Strategy (Phase-Based Rollout)

### **Phase 1A (Q4 2025) - NCR Flagship**
**Target:** Delhi metro area  
**Cities:** Delhi, Ghaziabad, Faridabad  
**Product:** Premium Tier (₹18-22K, all features + WiFi)  
**Rationale:** Largest population + worst pollution + highest purchasing power

### **Phase 1B (Year 2) - NCR Expansion**
**Target:** Extended metro + corporate hubs  
**Cities:** Noida, Gurugram, Baghpat, Greater Noida  
**Product:** Premium + Essential Tiers (Tier 2 without WiFi for price-sensitive segments)

### **Phase 2 (Year 2-3) - Regional Clusters**
**Target:** Tier-1 cities, industrial zones  
**Cities:** Patna (2.8M), Muzaffarpur, Bhiwadi (industrial), Singrauli  
**Product:** Essential Tier (₹12-15K, core features only)

---

## 📦 Product Recommendation Summary

### **Must-Have Core Features** (Validated by Analysis)
| Feature | Why It's Critical | Impact |
|---------|------------------|--------|
| **True HEPA H13** | PM2.5 in 73% of bad days | Essential filtration standard |
| **Pre-filter (washable)** | Extends HEPA life in dusty NCR | Cost optimization for users |
| **Activated Carbon** | O3 + odor control (traffic/cooking) | Holistic air quality improvement |
| **PM2.5 Sensor + Auto Mode** | AQI swings 34-42 points daily | Responsive to real-time pollution |
| **High CADR (350+ m³/h)** | Winter AQI 284 demands speed | Covers 350-500 sq ft effectively |
| **Sleep Mode + Timer** | 81% of winter nights need operation | User convenience + energy savings |
| **Seasonal Presets** | Winter (81%) vs Summer (41%) vs Monsoon (22%) | Adapt performance to real demand patterns |

### **Pricing Strategy**
- **Premium Tier:** ₹18-22K (WiFi app + all features) → NCR launch
- **Essential Tier:** ₹12-15K (core + manual control) → Year 2+ expansion
- **Filter Replacement:** ₹2,500-3,500 per 6-8 months → 60%+ attachment rate expected
- **3-Year LTV:** ₹6,000-7,000 per customer (recurring revenue potential)

---

## 📈 Success Metrics & Projections

**Phase 1 Goal (Year 1):**
- **5,000 units** in NCR (achieves 0.02% penetration of Delhi's 22M population)
- **CAC Target:** <₹2,000 (pre-winter digital campaigns)
- **Filter Attachment Rate:** >60% within 8 months

**Addressable Market (NCR + Bihar):**
- High-risk population: ~32.4M people
- At 1% penetration: 324,000 potential units
- Revenue opportunity: ₹4-7B in unit sales + ₹800M+ in recurring filters

---

## 📊 Interactive Dashboard

Explore the complete analysis, city-by-city breakdown, and real-time trends:

**[🔗 View Full Dashboard](https://lookerstudio.google.com/reporting/e16ab2ff-8c3e-46c8-a4eb-3c3d1ffb264b)**

The dashboard includes:
- Live AQI trends by city and season
- Priority city risk scores
- Competitor feature comparison
- Seasonality patterns and bad-air-day forecasts
- Market size and penetration scenarios

---

## 📁 Project Structure

```
Product-Market-Fit-Analysis---Case-Study/
├── README.md                                    # This file
├── Product Requirements Document.md             # Detailed product specs & BOM
├── problem_statement.pdf                        # Initial brief
├── Primary_and_Secondary_Analysis.pdf           # Research findings
│
├── SQL_Questions/
│   ├── Exploratory_Analysis.ipynb              # AQI trends, city rankings, pollutant analysis
│   ├── Dashboard Data Sources.ipynb            # Master dataset preparation
│   ├── master_dashboard_dataset.csv            # Processed data for visualizations
│   └── main.db                                 # DuckDB database with all queries
│
├── Dataset/                                     # Raw data sources
│   ├── air_purifier_search_trend_data.csv      # Google search trends for air purifiers
│   ├── day-wise-state-wise-air-quality-index-aqi-of-major-cities-and-towns-in-india.csv
│   ├── indian_cities.csv                       # Census 2011 city population data
│   ├── master-data-state-district-and-disease-wise-cases-and-death-reported-due-to-outbreak-of-diseases-as-per-weekly-reports-under-idsp.csv
│   └── master-data-state-vehicle-class-and-fuel-type-wise-total-number-of-vehicles-registered-in-each-month-in-india.csv
│
└── Output_Dataset/                              # Analysis results
    ├── priority_cities.csv                      # Top 12 cities ranked by risk score
    ├── aqi_seasonality.csv                      # Bad days % by season & city tier
    └── competitor_features_matrix.csv           # Feature comparison with 5 competitors
```

---

## 🔬 Analysis Highlights

### Pollutant Frequency (Bad Air Days Only)
**Top 5 Pollutants:**
1. PM2.5 (73% of incidents)
2. PM10 (68% of incidents)
3. O3 (Ozone - 3% of incidents)
4. CO (Carbon Monoxide - 2% of incidents)
5. SO2 (Sulfur Dioxide - 1% of incidents)

**Implication:** PM2.5 filter is non-negotiable; carbon layer covers ozone + odors.

### Top 5 Priority Cities (Risk Score Ranked)
| Rank | City | State | Pop (M) | Bad Days | Avg AQI | Score |
|------|------|-------|---------|----------|---------|-------|
| 🥇 | Delhi | Delhi | 22.0 | 51% | 216 | 36.8 |
| 🥈 | Ghaziabad | UP | 3.1 | 49% | 213 | 33.1 |
| 🥉 | Bhiwadi | Rajasthan | 0.14 | 49% | 206 | 32.2 |
| 4 | Greater Noida | UP | 0.13 | 47% | 206 | 31.4 |
| 5 | Faridabad | Haryana | 2.1 | 45% | 200 | 30.3 |

---

## 🎓 Key Learnings & Recommendations

✅ **Validated:** Year-round air purifier demand (not seasonal)  
✅ **Validated:** Strong NCR market concentration (pollution + purchasing power)  
✅ **Validated:** PM2.5 filtration as primary differentiator  
✅ **Confirmed:** Seasonal preset features add real value (81% winter vs 41% summer)  

💡 **Strategic Recommendations:**
1. **Launch winter Q4 2025** in Delhi to capture peak season demand
2. **Target pre-ordering in monsoon** (Q3 2025) to drive pipeline
3. **Partner with NCR e-commerce** (Amazon, Flipkart, local channels) for distribution
4. **Bundle replacement filters** in launch offer to build recurring revenue habit
5. **Emphasize summer/monsoon viability** in marketing to counter "seasonal product" perception


