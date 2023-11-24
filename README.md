# Water Quality Analysis 🚰💧

## Project Overview 🌐
Access to safe drinking water is crucial for health, a fundamental human right, and a key aspect of effective health protection policies. This data science project focuses on analyzing water quality and potability using a dataset that includes various metrics for 3276 different water bodies.

## Dataset 📊
The `water_potability.csv` file contains essential water quality metrics. Let's dive into the key parameters:

### 1. pH Value 📉
```python
# Load data
import pandas as pd
data = pd.read_csv('water_potability.csv')

# Analyze pH values
ph_values = data['ph']
ph_stats = ph_values.describe()

# Display statistics
print(ph_stats)

# Analyze hardness
hardness_values = data['hardness']
hardness_stats = hardness_values.describe()

# Display statistics
print(hardness_stats)
import matplotlib.pyplot as plt

# Plot pH values
plt.figure(figsize=(10, 6))
plt.hist(ph_values, bins=20, color='blue', alpha=0.7)
plt.title('Distribution of pH Values')
plt.xlabel('pH')
plt.ylabel('Frequency')
plt.show()

In this example, I've included a section for visualizations using matplotlib. You can customize the visualization code based on the type of plots you want to generate for your analysis. Simply replace the placeholder code with your actual code for generating visualizations.


