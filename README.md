This project is about predicting house prices using machine learning 🤖.
The goal is to understand how factors like income, number of rooms, and population affect house prices.

I built a model using Linear Regression that can estimate house prices based on these features.

***⚙️ What I Did***

✨ Cleaned the dataset  
✨ Handled outliers using IQR  
✨ Converted categorical data  
✨ Visualized data  
✨ Trained Linear Regression  
✨ Evaluated using MAE & R²  

***📊 Dataset***

The dataset includes:
🏘️ Area Income
🏡 House Age
🛏️ Number of Rooms
🛌 Number of Bedrooms
👥 Population
💰 Price (target)

***📈 Results***

✔ The model achieved an average error of around ₹82,000
✔ Predictions are very close to actual values
✔ The model shows good performance on test data

***📉 Visualizations****

🔹 Scatter Plot (Actual vs Predicted)

📌 Shows how close predictions are to real values

```python
plt.scatter(y_test, y_pred)
plt.xlabel("Actual Price")
plt.ylabel("Predicted Price")
plt.title("Actual vs Predicted Price")
plt.show()
```

🔹 Heatmap (Feature Correlation)

📌 Shows relationship between features

```python
sns.heatmap(df.corr(), annot=True)
plt.title("Correlation Heatmap")
plt.show()
```

🔹 Probability Distribution 📊

📌 Shows how data is distributed

```python
sns.kdeplot(df['Price'], fill=True)
plt.title("Price Distribution")
plt.show()
```

🔹 Bar Graph 📊

📌 Compare values easily

```python
sample = results.head(10)
sample.plot(kind='bar')
plt.title("Actual vs Predicted")
plt.show()
```

🔹 3D Plot 🌐

📌 Shows relationship between multiple features

```python
ax.scatter(df['Avg. Area Income'],
           df['Avg. Area Number of Rooms'],
           df['Price'])
```
           
***🔮 Future Improvements***

🚀 Use advanced models (Random Forest, XGBoost)
🚀 Add more real-world features
🚀 Use larger datasets
🚀 Deploy as a web application
