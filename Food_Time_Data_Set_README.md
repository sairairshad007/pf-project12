
# Food Time Data Set Limited

## Overview

The **Food Time Data Set Limited** gives information about food deliveries, focusing on the delivery staff, orders, weather, and traffic. You can use this dataset to analyze delivery times, improve logistics, or understand how different factors affect delivery operations.

## Data Structure

- Explain the format (rows, columns) and give a high-level view.

## Feature Descriptions

Detail each column in the dataset:

- Column Name: Description, Data Type, Example Values.
  
## Statistical Summary

- Provide key statistics like mean, median, min, and max for numerical data.

## Applications

List the possible uses of this dataset, e.g.:

- Predicting delivery times.
- Understanding traffic/weather impacts.

## File Contents

### Sheet: `secsheet`

This dataset includes the following information:

1. **ID**: A unique number for each record.
2. **Delivery_person_ID**: A unique ID for each delivery person.
3. **Delivery_person_Age**: The age of the delivery person.
4. **Delivery_person_Ratings**: Customer ratings for the delivery person (scale: 0 to 5).
5. **Restaurant_latitude**: The latitude of the restaurant.
6. **Restaurant_longitude**: The longitude of the restaurant.
7. **Delivery_location_latitude**: The latitude of the delivery location.
8. **Delivery_location_longitude**: The longitude of the delivery location.
9. **Type_of_order**: The type of food ordered (e.g., Snack, Drinks, Buffet).
10. **Type_of_vehicle**: The vehicle used for delivery (e.g., motorcycle, scooter).
11. **temperature**: The temperature during delivery (°C).
12. **humidity**: The humidity percentage during delivery.
13. **precipitation**: The amount of rain or snow (in mm).
14. **weather_description**: The weather condition (e.g., haze, mist).
15. **Traffic_Level**: The traffic conditions during the delivery (e.g., Low, High).
16. **Distance (km)**: The distance covered during the delivery (in kilometers).
17. **TARGET**: The delivery time goal (in minutes).

---

## Important Notes

- **Missing Data**: Some columns, like `Distance (km)`, may have missing values.
- **Units**:
  - Distances are in kilometers.
  - Temperature is in degrees Celsius.
  - Delivery time (`TARGET`) is in minutes.
- **Categories**: Columns like `Type_of_order`, `Type_of_vehicle`, and `Traffic_Level` have specific categories (e.g., "Snack," "High").
- **Location Data**: Latitude and longitude show the delivery route locations.

---

## Possible Uses

1. **Study Delivery Times**:
   - Find out what factors affect delivery times (e.g., traffic, weather).
2. **Improve Customer Experience**:
   - See how delivery ratings relate to delivery times or conditions.
3. **Optimize Delivery Routes**:
   - Analyze vehicle types and route distances to save time and fuel.
4. **Understand Weather Impact**:
   - Check how weather affects delivery operations.

---

## How to Use

1. **Load the Data**: Use Python to load the dataset:

   ```python
   import pandas as pd
   data = pd.read_excel("MY_project.xlsx", sheet_name="secsheet")
   ```

2. **Handle Missing Data**: Fill or remove missing values in columns like `Distance (km)` before analyzing.
3. **Create Visuals**: Use tools like matplotlib or seaborn to make graphs and charts.

---

## Acknowledgments

This dataset is for learning and analysis. Be careful with sensitive data (like location details) when sharing or using it.
