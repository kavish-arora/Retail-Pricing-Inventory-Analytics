# Retail Pricing & Inventory Analytics

Analysis of 3,700+ Zepto products to understand pricing strategies, stock levels, and discount effectiveness across categories.

## 🎯 Objectives
- Analyze pricing strategies and discount patterns
- Identify stock level issues and out-of-stock products
- Find best-value categories through price-per-weight analysis
- Highlight high-discount, low-stock problem products

## 🛠️ Tools Used
- **Python**: pandas, matplotlib, seaborn for data analysis
- **SQL**: Product segmentation, discount calculations, inventory filtering
- **Excel**: Data validation and reporting

## 📊 Key Findings
- Identified best-value categories with optimal discount rates
- Found correlation between high discounts and low stock levels
- Mapped frequently out-of-stock items impacting customer experience
- Discovered price-per-weight patterns for value assessment

## 🔧 Key SQL Queries

**Product Segmentation:**
```sql
SELECT category, AVG(discount_rate), COUNT(*) 
FROM products 
GROUP BY category;
```

**Problem Products:**
```sql
SELECT product_name, discount_rate, stock_level
FROM products 
WHERE discount_rate > 25 AND stock_level < 10;
```

## 📈 Business Impact
- Optimize inventory for high-discount, low-stock products
- Leverage best-value categories for promotions
- Improve supply chain planning for out-of-stock items

## 🚀 Usage
```bash
git clone [repository-url]
pip install pandas matplotlib seaborn
jupyter notebook analysis.ipynb
```

---
*Comprehensive retail analytics providing actionable insights for pricing optimization and inventory management.*
