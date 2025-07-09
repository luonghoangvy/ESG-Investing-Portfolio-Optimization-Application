# ESG Portfolio Optimization – Vietnam Sustainability Index (VNSI) Application
This project applies ESG-valued portfolio optimization to four Vietnamese stocks listed on the Vietnam Sustainability Index (VNSI). It combines traditional financial return models with sustainability (Environmental, Social, Governance) scores to evaluate risk-adjusted performance with ESG preference levels.
>  Authors: Luong Hoang Vy, Dao Thu Huyen, Bui Thi Yen Loan, Bui Thi Thanh Mai

---
## I. INTRODUCTION

### Problem Statement

In traditional finance, portfolios are optimized to maximize return and minimize risk. However, sustainability-conscious investors often seek portfolios that also align with environmental, social, and governance (ESG) values. This project aims to:

- Integrate ESG scores into portfolio return calculations using a λ-weighted utility function.
- Evaluate how ESG preferences (λ) and risk aversion (α) affect optimal asset allocation.
- Visualize ESG-efficient frontiers across different investor types.
---

## II. DATA OVERVIEW

- **Assets Used** (Vietnam VNSI stocks):
  - `FPT.VN` – FPT Corporation  
  - `VNM.VN` – Vinamilk  
  - `GEG.VN` – Gia Lai Electricity  
  - `VIC.VN` – Vingroup

- **Data Sources**:
  - Stock prices: Yahoo Finance (Nov 1, 2023 → Nov 1, 2024)
  - ESG scores: Normalized scores from VNSI

- **Variables**:
  - Daily returns \( r_{i,t} \)
  - ESG score \( \delta_i \) scaled to [-1, 1]
  - Combined ESG-valued return \( \zeta_{i,t}(\lambda) \)

## III. METHODOLOGY

### 1. ESG-Valued Return Formula:

![image](https://github.com/user-attachments/assets/fed0ce04-caba-45f5-a38a-2e3579c2da4f)


Where:
- \( \lambda \in [0, 1] \): investor’s ESG preference  
- \( c \): scaling constant  
- \( \delta_i \): ESG score  
- \( r_{i,t} \): daily financial return


### 2. Portfolio Optimization Objective:
![image](https://github.com/user-attachments/assets/ddc4867a-eb02-4d16-b915-ed88f8ce0dce)
