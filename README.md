# ShopSmart-E-commerce-Conversion-Predictor
📌 Project Overview
ShopSmart is a predictive analytics project designed to identify high-intent shoppers on e-commerce platforms. By analyzing 12,000+ session records, this project builds a machine learning pipeline to predict whether a visitor will generate revenue based on their browsing behavior and session attributes.

🛠️ Technical Stack
Language: Python

Data Manipulation: Pandas, NumPy

Machine Learning: Scikit-Learn (Decision Tree Classifier)

Visualization: Matplotlib, Seaborn

🚀 Key Engineering Workflow
1. Data Preprocessing & Transformation
Categorical Encoding: Used LabelEncoder to transform features like Month and VisitorType into numerical formats suitable for machine learning.

Type Casting: Converted Boolean indicators (Weekend, Revenue) into float types to ensure model compatibility.

Data Integrity: Handled missing values and verified data types using Pandas.

2. Exploratory Data Analysis (EDA)
Visualized revenue distribution to understand class imbalance.

Analyzed behavioral trends like shopping patterns on weekends vs. weekdays and the impact of different visitor types on conversion.

3. Model Engineering & Optimization
Algorithm: Implemented a Decision Tree Classifier.

Hyperparameter Tuning (Pre-pruning): Conducted a systematic search for the optimal max_depth (testing depths 2-10).

Optimization Result: Identified Depth 3 as the optimal balance between bias and variance, preventing overfitting while maintaining high predictive power.

4. Performance Metrics
Focused on the F1-Score as the primary evaluation metric to account for the imbalance in purchase events.

Final F1-Score: ~0.6436

5. Model Interpretability
Generated a Decision Tree Visualization to map out the decision-making logic of the model.

Identified PageValues as a critical feature in determining user purchase intent.

📈 Key Insights
Visitors with higher PageValues are significantly more likely to complete a transaction.

New visitors often show different conversion patterns compared to returning visitors, which the model successfully captures.

├── shop_smart_ecommerce.csv    # Raw dataset
├── ShopSmart_Project.ipynb      # Complete Jupyter Notebook
└── README.md                    # Project documentation
