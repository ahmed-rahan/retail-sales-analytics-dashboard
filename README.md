# 📊 Retail Sales Analytics Dashboard

![Project Status](https://img.shields.io/badge/Status-Complete-success)
![Python](https://img.shields.io/badge/Python-3.12-blue)
![SQL](https://img.shields.io/badge/SQL-Server-red)
![Excel](https://img.shields.io/badge/Excel-Advanced-green)

Automated sales analytics solution that processes 10,000+ retail transactions using Python, SQL, and Excel, reducing manual reporting time by 65%.

---

## 🎯 Project Overview

This project demonstrates end-to-end data analytics skills including data collection, cleaning, SQL querying, automation, and dashboard visualization. Built to showcase skills applicable to business intelligence, service operations analytics, and data-driven decision making.

**Key Achievement:** Reduced weekly reporting time from 30 minutes to 10 minutes (65% efficiency gain) through automated data processing pipeline.

---

## 📈 Business Impact

- ✅ **10,000+ transactions** processed and analyzed
- ✅ **65% time reduction** through Python automation
- ✅ **8% revenue recovery opportunity** identified through category analysis
- ✅ **4 interactive visualizations** for stakeholder insights
- ✅ **Production-ready** automated refresh system

---

## 🛠️ Technologies Used

### Programming & Data Processing
- **Python 3.12** - Data cleaning, transformation, and analysis
  - Pandas - Data manipulation and ETL pipeline
  - Matplotlib - Data visualization
  
### Database & Querying
- **SQL Server** - Structured data storage and querying
  - Advanced queries with CTEs, subqueries, aggregations
  - 8 production-ready analytical queries

### Visualization & Reporting
- **Excel** - Interactive dashboard creation
  - Pivot tables and dynamic charts
  - Advanced formulas and KPI tracking
  - 4-chart dashboard layout

### Automation
- **Python Scripts** - Automated weekly data refresh
- **Process Optimization** - Workflow automation

---

## 📊 Key Features

### 1. Automated ETL Pipeline
- Processes 540,000+ raw transactions
- Cleans and validates data (removes 135,000 invalid records)
- Filters to most recent 10,000 transactions for analysis
- Automated weekly refresh capability

### 2. SQL Database Integration
- Structured database (RetailSalesDB) with 10,000 records
- 8 analytical queries covering:
  - Revenue analysis by product and category
  - Daily sales trends
  - Geographic performance (country-level)
  - Underperforming category identification
  - High-value transaction analysis

### 3. Interactive Excel Dashboard
- **Key Metrics:** Total revenue, transactions, average order value, date range
- **Visualizations:**
  - Top 10 products by revenue (bar chart)
  - Daily sales trend (line chart)
  - Category performance (column chart)
  - Revenue by country (pie chart)

### 4. Business Insights
- Identified top-performing product categories (PAPER: 44% of revenue)
- Found 2 underperforming categories representing 8% revenue recovery opportunity
- Analyzed customer distribution across 5+ countries
- Tracked sales trends over 5-day period

---

## 📁 Project Structure
```
retail-sales-analytics/
│
├── scripts/
│   ├── analyze_sales.py          # Initial data analysis and cleaning
│   ├── auto_refresh.py            # Automated weekly refresh script
│   └── sales_analysis_queries.sql # SQL analytical queries
│
├── documentation/
│   ├── PROJECT_README.txt         # Detailed project documentation
│   ├── SQL_DOCUMENTATION.txt      # SQL queries reference
│   └── automation_log.txt         # Automation execution history
│
├── visualizations/
│   └── analysis_charts.png        # Python-generated charts
│
└── README.md                      # This file
```

---

## 🚀 How It Works

### 1. Data Collection & Cleaning
```python
# Load and clean raw data
df = pd.read_csv('data.csv', encoding='ISO-8859-1')
df = df.dropna(subset=['CustomerID'])
df = df[df['Quantity'] > 0]
df = df[df['UnitPrice'] > 0]
df['Revenue'] = df['Quantity'] * df['UnitPrice']
```

### 2. SQL Analysis
```sql
-- Top products by revenue
SELECT TOP 10
    Description,
    SUM(Revenue) as TotalRevenue,
    COUNT(*) as NumberOfOrders
FROM SalesTransactions
GROUP BY Description
ORDER BY TotalRevenue DESC;
```

### 3. Automated Refresh
- One-click Python script execution
- Updates all data files automatically
- Excel dashboard refreshes with new data
- Logs execution history for audit trail

---

## 💡 Key Insights

1. **Top Product:** PAPER CRAFT, LITTLE BIRDIE - $168,469 revenue (42.9% of total)
2. **Best Category:** PAPER products - $173,880 revenue (44.3% of total)
3. **Geographic Focus:** United Kingdom dominates sales
4. **Peak Period:** December 5-9, 2011
5. **Average Order:** $39.28 per transaction

**Revenue Recovery Opportunity:**
- Identified 2 underperforming categories
- Combined revenue: ~8% of total
- Recommendation: Optimize pricing, marketing, or inventory allocation

---

## ⚙️ Setup & Usage

### Prerequisites
```bash
pip install pandas matplotlib openpyxl
```

### Running the Analysis
```bash
# Initial analysis
python scripts/analyze_sales.py

# Weekly automated refresh
python scripts/auto_refresh.py
```

### SQL Queries
1. Open SQL Server Management Studio
2. Connect to server
3. Load `sales_analysis_queries.sql`
4. Execute queries for insights

### Dashboard
1. Open `sales_dashboard.xlsx`
2. Navigate to "Dashboard" sheet
3. Right-click any pivot table → Refresh
4. All charts update automatically

---

## 📊 Time Efficiency Metrics

| Process | Manual Time | Automated Time | Savings |
|---------|-------------|----------------|---------|
| Data Collection | 10 min | 2 min | 80% |
| Data Cleaning | 8 min | Auto | 100% |
| Excel Updates | 10 min | 5 min | 50% |
| Report Generation | 2 min | 3 min | -50% |
| **TOTAL** | **30 min/week** | **10 min/week** | **65%** |

**Annual Savings:** 17.3 hours/year per analyst

---

## 🎓 Skills Demonstrated

### Technical Skills
- Data cleaning and validation
- ETL pipeline development
- SQL database design and querying
- Advanced Excel (pivot tables, formulas, charts)
- Python programming (Pandas, Matplotlib)
- Process automation
- Data visualization

### Business Skills
- KPI identification and tracking
- Performance analysis
- Revenue optimization insights
- Stakeholder reporting
- Efficiency improvement (65% time reduction)

### Analytical Skills
- Trend analysis
- Category performance evaluation
- Customer segmentation
- Root cause analysis (underperforming categories)

---

## 🔮 Future Enhancements

Potential improvements for production deployment:

- [ ] Power BI migration for enhanced interactivity
- [ ] Real-time data integration via API
- [ ] Predictive analytics (sales forecasting)
- [ ] Customer segmentation analysis
- [ ] Automated email report distribution
- [ ] Mobile-responsive dashboard
- [ ] Multi-user access controls

---

## 📞 Contact

**Ahmed Rahan Kolikkara**
- 📧 Email: [rahan.kolikkara@gmail.com](url)
- 💼 LinkedIn: [https://www.linkedin.com/in/ahmed-rahan-k/](url)
- 🌐 Location: Dubai, UAE

---

## 📝 License

This project is available for portfolio demonstration purposes.

---

## 🙏 Acknowledgments

Dataset sourced from Kaggle's Online Retail Dataset for educational and portfolio purposes.

---

**⭐ If you found this project interesting, please consider giving it a star!**


https://github.com/ahmed-rahan/retail-sales-analytics-dashboard
