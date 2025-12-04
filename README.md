# 🧼 FMCG Home Care Synthetic Dataset (2023–2025)

This repository contains a fully synthetic, analytics-ready FMCG Home Care dataset designed for practicing real-world data analysis across Sales, Trade Marketing, and Brand roles.

The dataset simulates raw ERP-style transactional data typically found in FMCG companies, including multi-line invoices, multi-SKU brands, realistic pricing structures, promotions, distributor mapping, and seasonal effects.

> **Note:**  
> This dataset is entirely synthetic and **generated using ChatGPT**.  
> It does not represent any real company, customer, or commercial activity.

---

## 📦 Dataset Structure

### 1. `product_master.csv`
Contains product-level metadata:
- `sku_id`
- `brand`
- `sku_name`
- `pack_size`
- `channel_master` (MT / GT / Both)

### 2. `outlet_master.csv`
Contains outlet-level information:
- `outlet_id`
- `outlet_name`
- `channel` (MT / GT)
- `province`
- `distributor_id`

### 3. `distributor_master.csv`
Distributor overview including:
- `distributor_id`
- `distributor_name`
- `province_coverage`
- `historical_revenue`
- Pareto segmentation (top contributors)

### 4. `promo_master.csv`
Promo definitions:
- `promo_id`
- `promo_name`
- `promo_type` (Discount, Trade, Bundling, Multi-buy)
- `start_date`, `end_date`
- `channel_scope`
- `scope_type` (Global, Region, Distributor, Distributor_Segment)
- `discount_rate`
- `promo_budget`
- `listing_fee`

### 5. `sales_transactions.csv`
Daily line-item sales data (Jan 2023–Nov 2025):
- `transaction_id`
- `date`
- `outlet_id`, `outlet_name`
- `channel`, `province`, `distributor_id`
- `sku_id`, `sku_name`, `brand`, `pack_size`
- `qty`
- `unit_price`
- `sales_value`
- `promo_id`
- `discount_rate`
- Seasonal tagging (Ramadhan, Chinese New Year, Christmas, Harbolnas, Normal)

This dataset is structured to resemble realistic FMCG sales transactions pulled directly from ERP systems (SAP/Oracle/etc.), including multi-line invoice behavior.

---

## 🎯 Use Cases

This dataset is suitable for:

- Sales performance analysis  
- Trade marketing evaluation  
- Promo uplift analysis  
- Distributor segmentation (Pareto, regional, etc.)  
- Demand forecasting and 2026 target-setting  
- Price & discount behavior analysis  
- Brand and SKU performance measurement  
- Dashboard development (Looker Studio, Power BI, Tableau)  
- Machine Learning experiments on sales prediction

---

## ⚠️ Disclaimer

This dataset is **synthetic** and created solely for analytical practice.  
It does **not** reflect real business data.  
It was **generated using ChatGPT**.

