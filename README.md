# **Market Cycle Gene Forecasting Engine (MCGF)**

<p align="center">
  <img src="https://img.shields.io/badge/Language-Python_3.10+-blue?style=for-the-badge&logo=python">
  <img src="https://img.shields.io/badge/Focus-Tokenomic%20Forecasting-purple?style=for-the-badge">
  <img src="https://img.shields.io/badge/Analysis-Market%20Cycle%20Dynamics-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/Model-Trend%20%26%20MovingAverage-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/CLI-mcgf-9cf?style=for-the-badge">
  <img src="https://img.shields.io/badge/Research--Grade-yes-blueviolet?style=for-the-badge">
</p>

### *A Research Framework for Forecasting Tokenomic Gene Evolution Across Market Cycles*

---

# **Introduction**

The **Market Cycle Gene Forecasting Engine (MCGF)** is a research-oriented computational tool designed to analyze and forecast **tokenomic gene frequencies** across market cycles.

In modern tokenomics research, smart contract *features* minting logic, fee mechanisms, permission structures, risk vectors are treated as **economic “genes”**. These genes mutate, rise, fall, or completely disappear depending on:

* Market liquidity
* Narrative cycles
* Speculation waves
* Scam evolution patterns
* Behavioral incentives
* Developer trends

MCGF allows researchers to track these genes over time and **predict their future behavior** using lightweight, transparent, interpretable forecasting models.

Unlike AI-based predictors or noisy black-box tools, MCGF focuses on:

* clarity,
* interpretability,
* transparent assumptions,
* and reproducible analysis.

It is designed for economists, blockchain researchers, auditors, and anyone studying **tokenomics evolution as a scientific phenomenon**.

---

# **Theoretical Background**

## **Tokenomic Genes**

A *tokenomic gene* is a measurable behavior encoded in a smart contract.
Examples:

* `MINT_UNBOUNDED` | unlimited minting capability
* `FEE_BASIC` | simple transfer fees
* `FEE_HIGH_RISK_PATTERN` | scam-prone tax patterns
* `BLACKLIST_PRESENT` | selective transfer blocking
* `PROXY_UPGRADEABLE` | future mutation capability
* `REBASING_SUPPLY` | supply elasticity

Each gene is a **trait** that influences:

* economic incentives
* centralization level
* manipulation vectors
* user fairness
* systemic risk
* price dynamics

Gene frequencies across the ecosystem change over time and those changes correlate strongly with **market cycles**.

---

# **Market Cycles as Evolutionary Pressure**

MCGF is built on the observation that the crypto market behaves like an evolutionary environment:

### **Accumulation Phase**

* low liquidity
* low retail exposure
* high technical focus
* scam-genes suppressed
* governance/safety genes dominate

### **Early Bull Market**

* capital inflow
* creative experimentation
* new tokenomic patterns emerge

### **Late Bull Market**

* FOMO extremes
* rapid mutation
* scam-gene explosion (honeypots, dynamic-tax, mint exploits)

### **Bear Market**

* liquidity extinction
* predatory genes die off
* sustainable genes remain

MCGF helps quantify and **forecast** these evolutionary shifts.

---

# **Purpose of MCGF**

MCGF was designed to answer questions like:

* *Which tokenomic genes will dominate the next bull cycle?*
* *Are dangerous genes (honeypot patterns, blacklist logic) increasing or declining?*
* *How fast is a given gene evolving across cycles?*
* *Which tokenomic species are likely to re-emerge?*
* *How do different genes correlate with different market phases?*

This can support:

* academic research
* market intelligence
* scam prediction
* DeFi risk modeling
* tokenomics design
* macro-tokenomics forecasting

---

# **Forecasting Models**

MCGF includes two interpretable forecasting models:

---

## **1. Linear Trend Model (Default)**

Fits a simple regression:

```
frequency = a + b * time
```

This model is ideal for:

* steady gene drift
* macro-directional trends
* multi-cycle forecasting

Characteristics:

* interpretable
* stable
* transparent

---

## **2. Moving Average Model (MA)**

Computes the mean of the last `k` observations:

```
forecast = avg(last k frequencies)
```

Useful for:

* noisy data
* short-term smoothing
* low-variance genes

---

# **Features**

### Clean, professional, readable CLI

Perfect alignment, no Unicode issues, CMD-compatible.

### Interpretability-focused models

Preferable to “mystery-box” ML.

### Multi-gene dataset support

Analyze entire ecosystems at once.

### Phase-aware datasets

Compatible with annotated market cycles.

### Zero dependencies

Pure Python, portable and lightweight.

---

# **Project Structure**

```
market-cycle-gene-forecaster/
│
├── mcgf/
│   ├── cli.py               # CLI interface
│   ├── loader.py            # CSV parsing & grouping
│   ├── forecasting.py       # Trend & MA forecasting
│   └── models.py            # Data models
│
├── data/
│   └── gene_history_example.csv
│
├── README.md
└── pyproject.toml
```

---

# **Installation**

Inside the project directory:

```bash
pip install -e .
```

This registers the command:

```
mcgf
```

---

# **Usage**

### **Forecast future gene frequencies**

```bash
mcgf data/gene_history_example.csv
```

### **Predict a specific gene**

```bash
mcgf data/gene_history_example.csv --gene MINT_UNBOUNDED
```

### **Switch forecasting method**

```bash
mcgf data/gene_history_example.csv --method ma --window 3
```

### **Predict multiple steps ahead**

```bash
mcgf data/gene_history_example.csv --horizon 3
```

---

# **Example Output**

```
--------------------------------------------------------------------
 MARKET CYCLE GENE FORECAST – 1 STEP AHEAD  (method: trend)
--------------------------------------------------------------------

Total observations : 18
Total genes        : 3

Gene                         Last Freq     Forecast(+1)
--------------------------------------------------------------------
FEE_BASIC                      0.320         0.365
FEE_HIGH_RISK_PATTERN          0.210         0.236
MINT_UNBOUNDED                 0.120         0.138
--------------------------------------------------------------------

Done.
```

Professional. Clear. No Unicode issues.
Designed for CMD, PowerShell, macOS, Linux.

---

# **CSV Data Specification**

Each row represents a gene’s presence in a given time step:

```csv
time_index,phase,gene,frequency
1,accumulation,MINT_UNBOUNDED,0.02
2,accumulation,MINT_UNBOUNDED,0.03
3,early_bull,MINT_UNBOUNDED,0.05
...
```

Where:

| Field        | Description                    |
| ------------ | ------------------------------ |
| `time_index` | numeric chronological step     |
| `phase`      | market phase label             |
| `gene`       | gene identifier                |
| `frequency`  | normalized frequency (0.0–1.0) |

---

# **Research Applications**

### **1. Gene Drift Analysis**

Quantify how tokenomic genes mutate over time.

### **2. Scam Pattern Forecasting**

Predict the rise of dangerous patterns like:

* blacklist abuse
* dynamic tax scams
* honeypot structures

### **3. Tokenomics Evolution Modeling**

Identify which token species will re-emerge.

### **4. Market Intelligence**

Anticipate upcoming tokenomic trends in new cycles.

### **5. Academic Cryptoeconomics**

MCGF is suitable for:

* evolutionary economics papers
* on-chain behavioral analysis
* DeFi risk studies
* system dynamics modeling

---

# **Roadmap**

### Multi-horizon predictions (1, 3, 5, 10 steps)

### CSV + JSON export

### Correlation analysis between genes

### Market phase, conditioned models

### Volatility-adjusted forecasting

### Streamlit dashboard for visualization

### Integration with Token Genome Project datasets

### Evolutionary simulation engine

---

# **License**

MIT License, open for research, modification, and commercial use.

---

# **Contributing**

Contributions, new forecasting models, dataset expansions, and research collaborations are welcomed.

If you are working on:

* tokenomics
* gene drift
* smart-contract behavioral evolution
* on-chain economics
* DeFi risk modeling

your insights are extremely valuable.
