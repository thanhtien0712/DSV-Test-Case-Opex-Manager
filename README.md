# Test Case Analysis - Operational Excellence Manager (DSV x Schenker)

This repository contains the solutions and analysis report for the Operational Excellence Manager Test Case. It includes a visual HTML interface to detail the approach and problem-solving strategies used.

## 🚀 Key Contents

The project focuses on 2 main Case Studies:

### 1. Case Study 1: VBA Automation - Commodity Classification Tool
- **The Challenge:** Processing thousands of shipping records manually is prone to severe classification errors due to linguistic ambiguity in commercial documents (e.g., negation traps, substring conflicts, raw vs. finished goods).
- **The Solution:** Built a **Smart Classification Engine** using VBA.
  - **High Precision:** Prioritizes HS Code classification and uses user-defined exclusion lists (Dynamic Exclusions).
  - **Context Awareness:** Scans surrounding context (backward and forward) to detect negations or protect finished goods from being misclassified as raw materials.
  - **VBA Performance Optimization:** Ensures instantaneous execution by utilizing In-Memory Arrays, toggling environment settings (ScreenUpdating, Calculation), and dynamic filter cleansing.
  - **User Experience (UX):** Dynamically highlights matched keywords in red directly inside the text strings and outputs a detailed completion summary report.

### 2. Case Study 2: Data Management - Power Query & Power Pivot Solution
- **Data Schema:** Organized standard data structures using **Dimension Tables** (Lookup: Product_list, Customer_list) and **Fact Tables** (Event: Sales, Return).
- **Relationships (Data Model):** Established a rigorous Data Model with a strict 1-to-many filter flow (from Dim to Fact).
- **Transformation & DAX:** Implemented Calculated Columns (for Year and Quarter) and developed DAX Measures to power the final Pivot Table output.

## 🛠️ Tools & Technologies Used
- **Microsoft Excel:** VBA, Power Query, Power Pivot, DAX.
- **Frontend (Report Interface):** HTML, Tailwind CSS.

## 📂 How to Use
1. Open `Test Case Analysis.html` using any web browser (Chrome, Edge, Safari, etc.) to view the comprehensive presentation and features.
2. From the HTML page, you can click the **"Open File"** buttons to download or directly view the actual Excel/VBA solution files.
