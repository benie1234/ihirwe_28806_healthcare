Student Name:* Ihirwe Benie  
*Student ID:* 28806  
*Course:* INSY 8311 & Database Development with PL/SQL  
*Instructor:* Eric Maniraguha  



 Statement
This project system that helps pharmacies to manage their medicine stock in a smarter and faster way.
The system keeps track of medicine quantities, checks expiry dates, sends alerts, and predicts future demand using past data.
It reduces waste, avoids shortages, and protects patients from expired drugs.

 Objectives
- *Main Objective:* Build a normalized Oracle PL/SQL database to automate pharmacy inventory tracking, enforce drug safety rules, and predict future stock requirements.
- *Specific Objectives:*
  1. Design a 3rd Normal Form (3NF) relational database schema for suppliers, drugs, inventory batches, and sales.
  2.  to Write PL/SQL triggers to automatically block the sale of expired drugs and alert on low stock levels.
  3.  to Create PL/SQL procedures and packages for batch reception, sales processing, and inventory audits.
  4. to Develop an interactive dashboard to monitor expiry timelines and sales metrics in real time.

 Data Source
- *Dataset:* Pharma Sales and Drug Expiry Inventory Dataset (Kaggle)
- *Link:* https://www.kaggle.com/datasets

 Planned Tables
1. SUPPLIERS: Holds medicine supplier contact and license details.
2. MEDICINES: Central drug catalog detailing brand names, categories, and safety storage guidelines.
3. STOCK_BATCHES: Tracks batch numbers, quantity received, manufacture dates, and expiry dates.
4. CUSTOMERS: Stores customer/patient details for prescription verification.
5. SALES: Transaction headers recording total billing, dates, and customer details.
6. SALE_ITEMS: Line items linking specific drug batches to sales transactions.

Planned PL/SQL Features
- *Function (check_stock_level):* Returns current available stock for a specific medicine across all unexpired batches.
- *Procedure (process_drug_sale):* Handles sales transactions and updates batch quantities automatically.
- *Trigger (prevent_expired_sale):* A BEFORE INSERT trigger on SALE_ITEMS that blocks any attempt to sell a drug batch past its expiration date.
- *Package (pharmacy_inventory_pkg):* Consolidates all inventory management, expiry alert routines, and batch updates into one encapsulated unit.

Innovation
- *Option:* Analytics Dashboard
- *Tool:* Power BI / Streamlit
- *Description:* A live visual dashboard connected to Oracle database views displaying stock depletion trends, upcoming drug expiries (30/60/90 days), and high-demand medicine analytics.

## References
- Breen, L., & Smith, M. (2019). Secondary data analysis of inventory management in hospital and retail pharmacy environments. Journal of Health Organization and Management, 33(4), 412-428.
- World Health Organization. (2022). Substandard and falsified medical products and inventory wastage report. WHO.
- Oracle Corporation. (2024). Oracle Database PL/SQL Language Reference. Oracle Docs.
