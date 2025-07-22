# ⛎ Multi-Product-Production-Planning-using-Excel-Solver [Simplex-LP]
This repository represents a Gourmet Food Manufacturing co., a medium-sized specialty food processor facing complex production planning decisions across five product lines with multiple resource constraints

---

## ♊️ Executive Summary
Gourment Foods Manufacturing co., a medium-sized specicalty food processor facing complex production planning decisions across five product lines with multiple resource constraints. The optimization reveals surprising, counterintuitive results that demonstrate the powerful analytical capabilities of Excel Solver in unconvering non-obvious production strategies that maximize profitability

---

## 〽️ Company Profile: Gourmet Foods Manufacturing Co.
**Industry**: Specialty Food Processing
**Challenge**: Optimize monthly production mix across five premium products
**Objective**: Maximize total monthly profit while managing multiple resource constraints
**Complexity**: 5 Products, 5 Resource Constraints, non-intuitive optimal solution

### Product Portfolio
|*Product*|*Profit/Unit*|*Labor Hours*|
|---------|-------------|-------------|
|Premium Pasta Sauce|$12.5|0.15|
|Organic Honey|$8.25|0.1|
|Artisan Bread Mix|$6.75|0.08|
|Gourment Olive Oil|$18.9|0.2|
|Premium Vinegar|$14.6|0.18|

### Monthly resource constraints
- **Labour Hours**: 4500 hours available
- **Machine Time**: 2800 hours available
- **Tomatoes**: 6000 kg available
- **Herbs & Spices**: 3500 kg available
- **Production Budget**: $120000 available

### Linear Programming Model Formulation
#### Decision Variables
- **X₁** = Monthly production of Premium Paste Sauce
- **X₂** = Monthly production of Organic Honey
- **X₃** = Monthly production of Artisan Bread Mix
- **X₄** = Monthly production of Gourment Olive Oil
- **X₅** = Monthly production of Vinegar

#### Objective function
Maximize: 12.5X₁ + 8.25X₂ + 6.75X₃ + 18.9X₄ + 14.6X₅

#### Constraints
-         Labor: 0.15X₁ + 0.1X₂ + 0.08X₃ + 0.2X₄ + 0.18X₅ ≤ 4500
-       Machine: 0.08X₁ + 0.05X₂ + 0.06X₃ + 0.12X₄ + 0.1X₅ ≤ 2880
-      Tomatoes: 0.75X₁ + 0X₂ + 0X₃ + 0X₄ + 0X₅ ≤ 6000
-      Herbs & Spices: 0.12X₁ + 0.02X₂ + 0.35X₃ + 0.08X₄ + 0.15X₅ ≤ 3500
-        Budget: 3.8X₁ + 4.1X₂ + 2.25X₃ + 8.5X₄ + 5.2X₅ ≤ 120000

#### Production Bounds:
- 500 ≤ X₁ ≤ 8000
- 800 ≤ X₂ ≤ 12000
- 1000 ≤ X₃ ≤ 15000
- 300 ≤ X₄ ≤ 5000
- 400 ≤ X₅ ≤ 7000


