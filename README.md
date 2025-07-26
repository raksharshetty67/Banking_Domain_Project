# Banking Dashboard Project

# Overview
The Banking Dashboard Project is a data-driven initiative designed to analyze and visualize customer banking data, including deposits, loans, and account balances. Built using Python with libraries such as Pandas, Matplotlib, Seaborn, SQLAlchemy, and PyMySQL, alongside Power BI for advanced data visualization, this project transforms raw data from an Excel file into a MySQL database and generates both interactive visualizations in Jupyter Notebook and a dynamic, user-friendly dashboard in Power BI. These dashboards present key financial metrics and trends to assist financial analysts, bank managers, and data scientists in making informed decisions.

# Features

### Data Ingestion and Database Management

- Imports customer data from an Excel file into a MySQL database.
- Creates a banking database and `Customer` table using SQLAlchemy.

### Exploratory Data Analysis (EDA)

- Correlation analysis on numerical columns (e.g., Bank Deposits, Checking Accounts, Loans).
- Heatmap visualization of correlation coefficients.

### Interactive Dashboard

- Visual breakdowns of deposits, loans, savings, credit cards, and business lending.
- Pie charts for income band distribution.
- Bar charts for categorical comparisons (nationality, occupation, banking relationship).

### Scalability

- Easily extendable to new data sources and metrics.
- Supports filtering and segmentation for deeper insights.

# Prerequisites

## Software

- Python 3.11 or higher (recommended environment: Anaconda)
- MySQL Server (default: 127.0.0.1:3306)
- Power BI Desktop

### Python Libraries

- `mysql-connector-python`
- `pymysql`
- `sqlalchemy`
- `pandas`
- `matplotlib`
- `seaborn`



## Project Structure

```plaintext
├── Untitled (14).ipynb          # Main Jupyter Notebook
├── README.md                    # Documentation file
├── data/
│   └── customer_data.xlsx       # Excel data file
├── images/
│   ├── deposit_analysis.png
│   └── loan_analysis.png
└── video/
    └── banking_dashboard_demo.mp4  # (Optional) Demo video
```

---

## Data Description

### Demographic Data

- **Client ID**: Unique ID (e.g., IND81288)
- **Name**: Customer full name
- **Age**: Age of the customer
- **Location ID**: Geographical location code
- **Joined Bank**: Joining date (e.g., 06-05-2019)
- **Banking Contact**: Bank representative
- **Nationality**: e.g., American, African, European
- **Occupation**: e.g., Software Consultant, Technician

### Financial Metrics

- **Estimated Income**
- **Superannuation Savings**
- **Credit Card Balance**
- **Bank Loans**
- **Bank Deposits**
- **Checking Accounts**
- **Saving Accounts**
- **Foreign Currency Account**
- **Business Lending**

### Additional Data

- **Properties Owned**
- **Risk Weighting**
- **BRId**: Banking Relationship ID
- **GenderId**: Gender (1 for Female, 2 for Male)
- **IAId**: Institution Advisor ID
- **Fee Structure**: High, Mid, Low
- **Loyalty Classification**: Jade, Gold, Silver, Platinum

---

## Detailed Analysis and Insights

### Correlation Matrix

- **Bank Deposits** and **Checking Accounts** → Strong Positive Correlation
- **Bank Deposits** and **Saving Accounts** → High Savings Preference
- **Bank Deposits** and **Foreign Currency Account** → International Activity

These insights guide marketing and cross-selling strategies.

### Dashboard Breakdowns

- **Total Deposits**: 20.51M  
  - Bank Deposits: 10.51M  
  - Savings: 4.27M  
  - Checking Accounts: 5.28M

- **Total Loans**: 4.38bn  
  - Bank Loans: 1.77bn  
  - Business Lending: 2.60bn  
  - Credit Cards: 9.53M

- **Income Bands**:  
  - Low: 30.72%  
  - Medium: 19.72%  
  - High: 49.56%

- **Deposit by BR ID**: Highest in BRId 1
- **Deposit by Occupation**: Decreasing trend by profession
- **Deposit by Nationality**: Visual distribution across nationalities

---

## Screenshots

(Add images inside `images/` directory and embed them using:)

```markdown
![Deposit Analysis](images/deposit_analysis.png)
![Loan Analysis](images/loan_analysis.png)
```

---

## Video Demo

Watch the demo:  
`video/banking_dashboard_demo.mp4` *(Embed if uploaded to YouTube or elsewhere)*

---

## Potential Enhancements

- Real-Time Data Integration with Live MySQL
- More Visualizations (e.g., Line charts, scatter plots)
- Interactive Dashboard with **Plotly/Dash**
- Predictive Modeling (e.g., Loan default risk)
- Export Functionality (CSV, PDF)

---

## Troubleshooting

| Issue | Fix |
|-------|-----|
| MySQL Connection Errors | Ensure server is running, check connection string, and firewall settings |
| Module Not Found | Use `pip list` to verify. Reinstall if missing |
| Data Loading Issues | Check Excel file format and column names |
| Visualization Errors | Ensure libraries match Python version. Use `pip install --upgrade matplotlib seaborn` |

---

## Contributing

1. Fork the repo
2. Create a feature branch:

   ```bash
   git checkout -b feature-name
   ```

3. Commit your changes:

   ```bash
   git commit -m "Add feature-name"
   ```

4. Push and create a pull request

---

## License

This project is licensed under the **MIT License** — see the `LICENSE` file for details.

---

## Acknowledgments

- Inspired by banking analytics needs.
- Powered by open-source tools: Pandas, Matplotlib, Seaborn.
- Special thanks to the **xAI** community for support.

---

## Contact

For questions or collaboration, reach out via the **GitHub Issues** page or email at:  
📧 [rakksharshetty67@gmail.com]
