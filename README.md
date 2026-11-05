# Macroeconomic Demand Planning: MLR Simulation Model
Multiple Linear Regression model to identify key macroeconomic drivers of demand for B2B industrial 


###  Project Overview
This project is a **Proof of Concept (PoC) simulation** designed to demonstrate advanced predictive analytics for a B2B Industrial Manufacturer (e.g., Heavy Construction Materials). Unlike local retail models driven by short-term anomalies, commercial B2B demand fluctuates based on broader national and macroeconomic health. 

To demonstrate how to strip human bias from the forecasting process, I engineered a simulated dataset and developed a **Multiple Linear Regression (MLR)** model. This model isolates the exact mathematical relationship between macroeconomic indicators and Total Sales Revenue, showcasing how to build objective, data-driven forecasting tools from scratch.

###  The Simulated Business Challenge
In B2B industrial manufacturing, relying strictly on historical sales (time-series) or gut-feeling sales forecasts often leads to massive overproduction or severe capacity constraints. I designed this simulation to answer a core corporate supply chain question: *Which macroeconomic factors actually drive our revenue, and by exactly how much?*

###  The Solution & Methodology
I engineered a statistical regression model evaluating multiple independent variables against the dependent variable (Total Sales Revenue). 

**The Variables Analyzed:**
* **(Y)** Total Sales Revenue (Dependent)
* **(X1)** Macro Consumption Index
* **(X2)** Average Material Price
* **(X3)** New Construction Starts
* **(X4)** Capital Spending

**The Process:**
1. **Data Engineering:** Constructed a realistic historical annual dataset tracking total revenue alongside simulated national economic health indicators.
2. **Regression Modeling:** Utilized Excel's Data Analysis Toolpak (`LINEST`) to execute a Multiple Linear Regression matrix.
3. **Variance Analysis:** Calculated the expected Predicted Sales against actuals to isolate the model's residual variance.

###  Key Results & Statistical Impact
The regression output demonstrates how to successfully translate abstract economic data into concrete coefficients for S&OP planning.

* **Model Strength ($R^2$):** **94.56%** (The model explains over 94% of the variance in Total Sales Revenue).
* **Adjusted R-Squared:** **93.35%** (Confirming the model is appropriately fitted and not simply over-indexed on too many variables).
* **Identifying True Key Drivers (P-Value Analysis):** By analyzing the P-values against a standard 95% confidence threshold ($p < 0.05$), I was able to mathematically prove which variables actually move the needle versus which are just noise:
  * **New Construction Starts (X3):** The absolute strongest driver in the model ($p = 0.000007$). Highly statistically significant.
  * **Average Material Price (X2):** A confirmed, significant driver of total revenue ($p = 0.0129$).
  * **Consumption (X1) & Capital Spending (X4):** Both returned P-values just above the threshold ($p = 0.053$ and $p = 0.062$, respectively), indicating they are secondary, borderline factors rather than primary baseline drivers.
* **Business Application:** This framework demonstrates how to shift a corporate S&OP discussion from subjective sales team estimates to objective, quantifiable economic realities.

###  Tools & Skills Demonstrated
* **Advanced Excel:** Data Analysis Toolpak, `LINEST` matrix functions, Variance Calculation, and Statistical Modeling.
* **Supply Chain & S&OP:** B2B Demand Planning, Macroeconomic Forecasting, and Objective Consensus Building.
* **Data Analytics:** Multiple Linear Regression (MLR), R-Squared interpretation, coefficient mapping, and predictive financial modeling.
