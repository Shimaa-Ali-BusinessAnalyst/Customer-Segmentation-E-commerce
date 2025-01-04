# Customer Segmentation E-commerce

This project applies K-Means clustering to segment customers based on their demographic and behavioral characteristics. These insights are used to guide targeted marketing strategies.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Cluster Insights](#cluster-insights)
5. [Key Visualizations](#key-visualizations)
6. [How to Use](#how-to-use)
7. [Tools Used](#tools-used)
8. [License](#license)

## Project Overview
Customer segmentation is essential for businesses to personalize their marketing strategies. This project identifies distinct customer groups based on their age, income, spending score, and gender. These clusters enable businesses to better understand and target specific customer segments for enhanced engagement.

## Dataset
- **Name**: `Mall_Customers.csv`
- **Features**:
  - `CustomerID`: Unique ID for each customer.
  - `Gender`: Male/Female.
  - `Age`: Customer's age.
  - `Annual Income (k$)`: Annual income in thousands.
  - `Spending Score (1-100)`: Spending behavior score.

The dataset is publicly available on Kaggle.

## Methodology
1. **Data Preprocessing**:
   - Checked for missing values and duplicates.
   - Scaled numerical features (Age, Annual Income, Spending Score) using StandardScaler.
2. **Clustering**:
   - Applied the K-Means clustering algorithm.
   - Determined the optimal number of clusters using the Elbow Method and Silhouette Score.
3. **Visualization**:
   - Enhanced visualizations for easier interpretation of clusters, including box plots, scatter plots, and pie charts.

## Cluster Insights
### Cluster 0: Moderate Income - Balanced Spenders
- **Characteristics**:
  - Annual income ~50k.
  - Balanced spending score (~50).
- **Interpretation**:
  - Likely represents middle-aged individuals with moderate income and spending. A balanced demographic in terms of financial activity.

### Cluster 1: High Income - High Spenders
- **Characteristics**:
  - High annual income (~80k).
  - High spending score (~80).
  - Typically younger customers.
- **Interpretation**:
  - Likely represents younger professionals or affluent individuals with high spending potential.

### Cluster 2: Low Income - High Spenders
- **Characteristics**:
  - Low income (~20k).
  - High spending score (~80).
- **Interpretation**:
  - Likely represents young individuals, possibly students or early-career professionals, who are enthusiastic about spending.

### Cluster 3: High Income - Low Spenders
- **Characteristics**:
  - High annual income (~80k).
  - Low spending score (~20).
- **Interpretation**:
  - Likely represents affluent individuals who prioritize saving over spending.

### Cluster 4: Low Income - Low Spenders
- **Characteristics**:
  - Low annual income (~20k).
  - Low spending score (~20).
  - Majority are older customers.
- **Interpretation**:
  - Likely represents individuals with lower income levels who spend conservatively.

## Key Visualizations
- **Scatter Plot**: Annual Income vs Spending Score
  ![Annual Income vs Spending Score](https://github.com/Shimaa-Ali-BusinessAnalyst/Customer-Segmentation-E-commerce/blob/main/Visualizations/Annual%20Income%20vs%20Spending%20Score.PNG)
  
- **Pie Chart**: Gender Distribution by Cluster
  ![Gender Distribution by Cluster](visuals/Gender_Distribution_by_Cluster.PNG)
  
- **Box Plot**: Age Distribution by Cluster
  ![Age Distribution by Cluster](visuals/Age_Distribution_by_Cluster.PNG)
  
- **Violin Plot**: Spending Score Distribution by Cluster
  ![Spending Score Distribution by Cluster](visuals/Spending_Score_Distribution_by_Cluster.PNG)

- **Violin Plot**: Annual Income Distribution by Cluster
  ![Annual Income Distribution by Cluster](visuals/Annual_Income_Distribution_by_Cluster.PNG)

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Customer-Segmentation-Analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Customer-Segmentation-Analysis
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Open `Mall Customer Segmentation.ipynb` to explore the analysis and visualizations.

## Tools Used
- **Python**: Programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Seaborn/Matplotlib**: Data visualization
- **Plotly**: Interactive visualizations
- **Scikit-learn**: Machine learning (K-Means clustering)

## License
This project is licensed under the MIT License. Feel free to use, share, or modify the code.

---
**Author**: Shimaa Ali  
**Portfolio**: [[Shimaa-Ali-BusinessAnalyst](https://github.com/Shimaa-Ali-BusinessAnalyst)]  
**LinkedIn**: [[Shaimaa-Ali](www.linkedin.com/in/shaimaa-ali33lux)]
