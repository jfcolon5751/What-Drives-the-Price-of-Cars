Detailed Report for Deployment: What Drives the Price of a car?

Objective
The purpose of this project is to provide the dealership with a analysis in detail about what drivers increase the price of use cars and how to make viable recomendations on inventory for used cars. The model leverages data-driven insights to predict the price of vehicles based on key attributes such as mileage, age, condition, fuel type, and drivetrain. This enables the dealership to make informed pricing decisions, optimize inventory, and improve customer satisfaction.

Model Overview Trained Models:

Linear Regression: Baseline model for transparency and interpretability.
Ridge Regression: Introduces regularization to reduce overfitting; selected hyperparameter alpha=10.
Lasso Regression: Adds sparsity by reducing the influence of less important features; selected hyperparameter alpha=0.1.
Evaluation Metrics:

Root Mean Squared Error (RMSE): $10,161
Average deviation of predicted prices from actual prices.
Penalizes larger errors more heavily, making it suitable for high-value predictions like car pricing.
Mean Absolute Error (MAE): $6,880
Provides a straightforward measure of the average error magnitude.
R² Score: ~53.2%
Explains approximately 53.2% of the variance in car prices, indicating that the model captures significant patterns in the data but has room for further improvements.
Selected Model:

Ridge Regression with alpha=10:
Chosen for its balance between performance and regularization.
Slightly edges out Linear Regression by handling multicollinearity more effectively.
Key Findings from Feature Analysis
The model reveals significant insights into factors that drive used car pricing:

Top Positive Influences on Price:
Diesel Fuel (+$13,451): Diesel cars are highly valued due to their fuel efficiency and durability.
New Condition (+$5,887): Cars in "new" condition command a substantial premium over others.
More Cylinders (+$2,408): Vehicles with more cylinders, typically associated with larger engines, are priced higher.
Four-Wheel Drive (4WD) (+$1,924): 4WD cars attract higher prices, reflecting their popularity for off-road and all-weather use.
Top Negative Influences on Price:
Odometer (Mileage) (-$6,529): Cars with higher mileage are devalued significantly, reflecting wear and tear.
Car Age (-$4,151 per standard deviation): Older cars naturally lose value over time.
Salvage Condition (-$2,452): Cars with a salvage title, indicating previous severe damage, are heavily devalued.
Gasoline Fuel (-$4,386): Gasoline cars are less valued compared to diesel and hybrid vehicles.
Features with Neutral or Minimal Influence:
Paint Color and Location (State): These features have negligible impact on pricing.
Model and Manufacturer: Minimal direct effect, as their influence is captured by other features like condition, fuel, and drivetrain.
Recommendations for Deployment
The dealership can leverage these insights to refine its operations and strategies:

1. Actionable Business Insights:
Customers appear to be driven to seek Fuel Type Diesel and 4WD Vehicles vehicles as a priority.  Diesel cars appear to demand a price premium, especially as fuel efficiency is prioritized.  All 4WD vehicles appeal to a broad market, including off-road enthusiasts and those in colder climates.

2. Seek Newer Cars with Lower Mileage. Customers appear to favor cars with lower mileage and there is a relationship with yielding higher prices and demand is higher to consumers.  Reframe from purchasing any vehicles with a Salvage Title as they tend to have low resale value.

3. Model Deployment Strategy: System Integration: Prioritize a Ridge Regression model in the dealership's  decision making process. Provide the entire team access to the input vehicle details seeking dynamic price recommendations.

4.  Web based Pricing Tool: Develop a web interface to enable real-time pricing predictions for both internal staff and potential buyers.

5. Maintenance and  Monitoring (After Implementation):
Produce a quaterly trailing 12 months of sales information and customer feedback. Update the systema and compared system predictions to actual to evalauate the model performance.  Monitore the system for market conditions not accounted into the model (Supply shortages, tarrifs of new inventories from outside countries)
Update the model as necessary for new market data.


Link to the Notebook
https://github.com/jfcolon5751/What-Drives-the-Price-of-Cars

