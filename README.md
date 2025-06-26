<h1>Telco Customer Churn - EDA Project</h1>
    <p>This repository contains an exploratory data analysis (EDA) of the Telco Customer Churn dataset. The objective is to understand customer behavior, identify patterns in churn, and explore features that influence customer retention.</p>

  <h2>📁 Dataset Overview</h2>
    <ul>
        <li><strong>Source</strong>: Telco Customer Churn dataset (Kaggle / IBM Sample Dataset)</li>
        <li><strong>Rows</strong>: 7,043 customers</li>
        <li><strong>Columns</strong>: 21 features</li>
        <li><strong>Target Column</strong>: Churn (Yes/No)</li>
    </ul>

  <p>Features include:</p>
    <ul>
        <li>Demographics: gender, SeniorCitizen, Partner, Dependents</li>
        <li>Services signed up: PhoneService, InternetService, StreamingTV, etc.</li>
        <li>Account details: tenure, Contract, PaperlessBilling, PaymentMethod</li>
        <li>Charges: MonthlyCharges, TotalCharges</li>
    </ul>

   <h2>🧹 Data Cleaning</h2>
    <ul>
        <li>Converted TotalCharges to numeric, handled invalid blanks</li>
        <li>Removed 11 rows with NaN in TotalCharges</li>
        <li>Reset index after dropping rows</li>
        <li>Encoded Yes/No columns into 1/0</li>
    </ul>

  <h2>📊 Exploratory Data Analysis (EDA)</h2>
    <ol>
        <li>Churn Distribution – 26.5% customers churned</li>
        <li>Gender-wise Churn – Similar churn rates</li>
        <li>Contract Type vs Churn – Month-to-month users churn more</li>
        <li>Monthly Charges vs Churn – Higher charges = more churn</li>
        <li>Tenure vs Churn – New customers churn more</li>
        <li>Internet Service vs Churn – Fiber users churn more</li>
        <li>Payment Method vs Churn – Electronic checks = high churn</li>
        <li>Correlation Heatmap – tenure & churn negatively correlated</li>
    </ol>

  <h2>📌 Key Insights</h2>
    <ul>
        <li>Long-term contracts reduce churn</li>
        <li>Higher bills and shorter tenure increase churn</li>
        <li>Fiber and electronic check users churn more</li>
    </ul>

   <h2>🛠 Tools Used</h2>
    <ul>
        <li>Python, Pandas, NumPy</li>
        <li>Seaborn, Matplotlib</li>
        <li>Jupyter Notebook</li>
    </ul>

  <h2>📂 Folder Structure</h2>
    <pre>
├── Telco_EDA.ipynb         # Main EDA notebook
├── telco_churn.csv         # Original dataset
├── graphs/                 # (Optional) Visuals exported
├── README.md
    </pre>

  <h2 id="contributing">🤝 Contributing</h2>
  <p>Contributions are welcome! Please fork the repository and submit a pull request.</p>

  <h2 id="license">📄 License</h2>
  <p>This project is open-source and available under the <strong>MIT License</strong>.</p>

  <h2 id="contact">📬 Contact</h2>
  <p>Created with ❤️ by <strong>Vansh Jain</strong> - feel free to reach out via <a href="mailto:vanshjainbro@gmail.com">Email</a> or connect on <a href="https://https://www.linkedin.com/in/vansh-jain-471145289/">LinkedIn</a>.</p>

