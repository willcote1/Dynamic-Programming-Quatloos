# Dynamic-Programming-Quatloos

To anyone insterested, these are the instructions. This project involves application of dynamic programming techniques:

## **Maximizing Money With Known Political Instability**

### **Political Landscape in Modora**
- Modora has **three political parties**:
  - **Plutocrats**: Favor the wealthiest third (≥ $1,000,000 quatloos).
  - **Revolutionaries**: Favor the poorest third (< $100,000 quatloos).
  - **Middletarians**: Favor the middle third ($100,000–$1,000,000 quatloos).
- **Government control schedule over the next 30 years**:
  - **Plutocrats:** Years **[0, 5)** and **[20, 25)**
  - **Revolutionaries:** Years **[5, 10)** and **[15, 20)**
  - **Middletarians:** Years **[10, 15)** and **[25, 30)**

---

### **Policies Under Each Party**
#### **Plutocrats' Policies**
- At the beginning of their rule:
  - Anyone **≤ $1,000,000** loses **$50,000** (or all if worth < $50,000).
  - Anyone **> $1,000,000** gains **$100,000**.

#### **Revolutionaries' Policies**
- At the start of years **5 and 15**:
  - Anyone **> $1,000,000** is reduced to **$10,000**.
  - Anyone **≤ $100,000** is boosted to **$1,000,000**.
- Progressive wealth reductions over four years:
  - Year 2: Those with **$900,000–$1,000,000** reduced to **$10,000**.
  - Year 3: Those with **$800,000–$900,000** reduced to **$10,000**.
  - Year 4: Those with **$700,000–$800,000** reduced to **$10,000**.
  - Year 5: **Everyone** gets **$100,000**.

#### **Middletarians' Policies**
- At the start of years **10 and 25**:
  - Anyone **> $1,000,000** loses **$900,000**.
  - Anyone **$100,000–$1,000,000** gains **$900,000**.

---

### **Annual Income and Investment Options**
- **Annual salary**: $60,000 **(received after financial policy changes)**.
- Choose **one** of four investments each year:
  1. **Fred’s Bank**: Gains **$40,000**.
  2. **The Bank of Marcus**: Loses **$90,000** (or all but $10 if worth < $90,010).
  3. **Bito Wladon’s Sound Investments**: Increases by **5%**.
  4. **Wellington Financial**: Decreases by **15%**.

---

### **Dynamic Programming Optimization**
- **Goal**: **Maximize wealth** at the end of **30 years**.
- **Use the provided code** (`Proj 3 Optimal Quatloos.ipynb`) to determine:
  1. **Maximum wealth and annual investment strategy** for:
     - **Initial wealth of $0**.
     - **Initial wealth of $50,000**.
     - **Initial wealth of $1,000,000**.
  2. **Recalculate with a new political schedule**:
     - **Plutocrats:** **[0, 5) and [20, 25)**
     - **Revolutionaries:** **[10, 15) and [25, 30)**
     - **Middletarians:** **[5, 10) and [15, 20)**

---

### **Submission Requirements**
1. **Submit two Jupyter Notebook files**:
   - `Proj 3 Optimal Quatloos 1.ipynb` (**Original government schedule**).
   - `Proj 3 Optimal Quatloos 2.ipynb` (**Revised government schedule**).
2. **Ensure your output includes**:
   - **Optimal final wealth**.
   - **Annual investment decisions**.
   - **Resulting financial trajectory (graphs and logs)**.
