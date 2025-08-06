# 📊 Sales Analytics Dashboard - Power BI Project

> **Comprehensive Business Intelligence Solution for Collectible Vehicle Sales Analysis**

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)](https://www.microsoft.com/en-us/microsoft-365/excel)

## 🚀 Project Overview

This Power BI dashboard provides comprehensive analytics for a specialized collectible vehicle and transportation equipment business, analyzing **$10.03M in revenue** across **2,823 transactions** from **2003-2005**. The project demonstrates advanced data visualization techniques and strategic business intelligence insights.

### 🎯 Key Metrics
- **Total Revenue:** $10.03 Million
- **Customer Base:** 92 Unique Customers
- **Geographic Reach:** 19 Countries
- **Product Categories:** 7 Distinct Lines
- **Order Fulfillment:** 92.7% Success Rate

---

## 📸 Dashboard Preview

### Business Overview Dashboard

<img width="1516" height="853" alt="Screenshot 2025-08-06 020117" src="https://github.com/user-attachments/assets/12e78d92-92ae-4dcf-8270-24a741702ac2" />

### Performance Analytics

<img width="1515" height="850" alt="Screenshot 2025-08-06 020134" src="https://github.com/user-attachments/assets/bc6eab82-f133-4fde-9f26-94a881170d46" />

### Customer Analytics

<img width="1513" height="850" alt="Screenshot 2025-08-06 020149" src="https://github.com/user-attachments/assets/cabd4fc5-c216-4911-b6a3-a040f86bb164" />

---


https://github.com/user-attachments/assets/2efead1c-9c8d-4767-a599-1db0057b239c


## 🛠️ Tech Stack

| Technology | Purpose | Version |
|------------|---------|---------|
| **Power BI Desktop** | Data Visualization & Dashboard Creation | Latest |
| **Microsoft Excel** | Data Source & Storage | 2019+ |
| **DAX** | Data Analysis Expressions | - |
| **Power Query** | Data Transformation | - |

---

## 📁 Project Structure

```
sales-analytics-dashboard/
│
├── 📊 Dashboards/
│   ├── Business-Overview.pbix
│   ├── Performance-Analytics.pbix
│   └── Customer-Analytics.pbix
│
├── 📈 Data/
│   ├── Sales.xlsx
│   └── data-dictionary.md
│
├── 📋 Documentation/
│   └── strategic-analysis-report.md
│
├── 🖼️ Screenshots/
│   ├── executive-dashboard.png
│   ├── performance-analytics.png
│   └── customer-intelligence.png
│
└── 📜 Scripts/
    ├── data-cleaning.pq
    └── dax-measures.txt
```

---

## 🎨 Dashboard Features

### 📊 **Executive Summary Page**
- **Revenue KPIs:** Total sales, profit margins, and growth trends
- **Operational Metrics:** Order fulfillment rates and average order values
- **Product Performance:** Revenue distribution across product lines
- **Pricing Analysis:** MSRP vs. Discounted vs. Premium positioning

### 📈 **Performance Analytics Page**
- **Time Series Analysis:** Monthly and yearly revenue trends
- **Product Line Comparison:** Performance across 7 categories
- **Seasonal Patterns:** Monthly sales fluctuations
- **Growth Indicators:** Year-over-year comparisons

### 👥 **Customer Intelligence Page**
- **Customer Segmentation:** Top customers by revenue contribution
- **Geographic Distribution:** Sales across 19 countries
- **Purchase Behavior:** Order patterns and customer lifetime value
- **Risk Analysis:** Customer concentration insights

---

## 🔍 Key Insights Discovered

### 💡 **Strategic Findings**
- **Customer Concentration Risk:** Top 3 customers represent 17.6% of total revenue
- **Product Performance Gap:** Classic Cars (39% revenue) vs. Trains (2.3% revenue)
- **Operational Excellence:** 92.7% shipping success rate indicates strong fulfillment
- **Market Opportunity:** Only 92 customers for $10M suggests expansion potential

### 📊 **Performance Highlights**
- **Highest Performing Product:** Classic Cars ($3.92M revenue)
- **Average Customer Value:** $109,120 per customer
- **Geographic Leader:** Strong international presence across 19 countries
- **Order Efficiency:** $3,554 average order value

---

## 🚀 Getting Started

### Prerequisites
- Power BI Desktop (latest version)
- Microsoft Excel 2019 or later
- Basic understanding of DAX and Power Query

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Ahmed-Esso/Sales-Analysis-Project.git
   cd sales-analytics-dashboard
   ```

2. **Open Power BI Files**
   ```
   Open Power BI Desktop
   File → Open → Select .pbix files from Dashboards folder
   ```

3. **Data Connection Setup**
   ```
   Ensure Sales.xlsx is in the correct path
   Refresh data connections in Power BI
   Update file paths if necessary
   ```

4. **Customize for Your Data**
   ```
   Replace sample data with your dataset
   Update DAX measures as needed
   Modify visualizations to match your requirements
   ```

---

## 📊 Data Schema

### Primary Dataset: `Sales.xlsx`

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| `ORDERNUMBER` | Integer | Unique order identifier |
| `QUANTITYORDERED` | Integer | Number of items ordered |
| `PRICEEACH` | Currency | Price per individual item |
| `SALES` | Currency | Total sales amount |
| `ORDERDATE` | DateTime | Date of order placement |
| `PRODUCTLINE` | Text | Product category |
| `CUSTOMERNAME` | Text | Customer company name |
| `COUNTRY` | Text | Customer country |
| `DEALSIZE` | Text | Order size category (Small/Medium/Large) |

**Total Records:** 2,823 transactions  
**Date Range:** 2003-2005  
**Geographic Coverage:** 19 countries

---

## 🎯 Business Impact

### 📈 **Measurable Outcomes**
- **Revenue Optimization:** Identified $700K+ opportunity through improved fulfillment
- **Risk Mitigation:** Highlighted customer concentration requiring diversification
- **Product Strategy:** Data-driven recommendations for portfolio optimization
- **Market Expansion:** Geographic analysis supporting international growth

### 💼 **Executive Value**
- **Strategic Planning:** Clear insights for business direction
- **Performance Monitoring:** Real-time KPI tracking
- **Risk Assessment:** Customer and product concentration analysis
- **Growth Opportunities:** Market expansion and product optimization

---

## 🔧 Advanced Features

### DAX Measures Implemented
```dax

AOV = DIVIDE([Total Sales], [Total Orders], 0)

Shipped Count = 
CALCULATE(
    COUNTROWS(Sales),
    Sales[STATUS] = "Shipped"
)

Shipped Percentage = 
DIVIDE(
    [Shipped Count],
    COUNTROWS(Sales)
)

Profit Margin = Sales[SALES] * 0.3 

Price Difference = Sales[PRICEEACH] - Sales[MSRP]
```

### Power Query Transformations
- Data type standardization
- Date parsing and formatting
- Geographic data cleansing
- Product categorization
- Customer name standardization

---

## 📱 Mobile Responsiveness

The dashboard is optimized for multiple viewing platforms:
- **Desktop:** Full feature experience with detailed analytics
- **Tablet:** Responsive layout with touch-friendly interactions  
- **Mobile:** Essential KPIs and simplified visualizations

---

## 🤝 Contributing

We welcome contributions to improve this dashboard! Here's how you can help:

### 🔄 **How to Contribute**
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### 📋 **Contribution Guidelines**
- Follow Power BI best practices for dashboard design
- Include documentation for new features
- Test all changes thoroughly
- Maintain consistent formatting and naming conventions

---

## 🐛 Known Issues & Limitations

### Current Limitations
- **Historical Data Only:** Dataset covers 2003-2005 period
- **Static Dataset:** No real-time data refresh capabilities
- **Limited Geographic Detail:** Country-level only, no regional breakdown
- **Product Hierarchy:** Single-level categorization

### Planned Improvements
- [ ] Real-time data integration
- [ ] Advanced geographic mapping
- [ ] Predictive analytics features
- [ ] Mobile app integration
- [ ] Automated report distribution

---

## 🏆 Acknowledgments

### 🙏 **Special Thanks**
- **Power BI Community** for best practices and inspiration
- **Microsoft Documentation Team** for comprehensive resources
- **Open Source Contributors** who make projects like this possible
- **Business Stakeholders** who provided requirements and feedback

### 📚 **Inspiration & References**
- [Power BI Dashboard Design Best Practices](https://powerbi.microsoft.com/en-us/blog/)
- [Business Intelligence Design Patterns](https://www.kimballgroup.com/)
- [Data Visualization Principles](https://www.storytellingwithdata.com/)

---

<div align="center">

### ⭐ **Star this repository if it helped you!** ⭐

**Built with ❤️ by Ahmed Essam | Powered by Power BI**

[⬆ Back to Top](#-sales-analytics-dashboard---power-bi-project)

</div>
