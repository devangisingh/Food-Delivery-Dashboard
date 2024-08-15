# Food-Delivery-Dashboard

## Objective
To design and implement an interactive Power BI dashboard that provides actionable insights into food delivery performance by analyzing key metrics such as orders, customer satisfaction, customer demographics, overall sales, food category and order trends. The dashboard aims to improve operational efficiency, identify bottlenecks, and support strategic decision-making by offering clear, data-driven visualizations that enable stakeholders to optimize delivery processes and enhance overall customer experience.

## Dataset
The dashboard utilizes five primary Excel datasets to provide a comprehensive analysis:
- **Food:** Contains details about individual food items available with their category & id. Key Fields: Food ID, Food Name and Category.

- **Users:** Includes information about the customers. Key Fields: User ID, Name, Age, Gender, Marital Status, Occupation and restuarant id.

- **Orders:** Records of each food order placed by users. Key Fields: Order Date, User ID, Restaurant ID, Quantity, Sales and Currency.

- **Restaurant:** Details about the restaurants participating in the food delivery service. Key Fields: Restaurant ID, Name, Location, Cuisine Type, Contact Information, and Ratings.

- **Menu:** Contains information about the menu items offered by each restaurant. Key Fields: Menu ID, Restaurant ID, Food ID, Menu Category, Price and Cuisine.

- **Data Relationships:**
1. Food and Menu: The Menu dataset links food items to specific restaurants.
2. Users and Orders: Orders are associated with users to track order history and customer behavior.
3. Restaurants and Orders: Orders are linked to restaurants to analyze performance and delivery metrics.
4. Menu and Orders: Orders linked to Menu describes what users ordered cusisine available in Menu.

## Methodology
- **Data Collection and Preparation:**
1. Data Sources: Collected data from various sources.
2. Data Cleaning: Cleaned the data by removing duplicates, handling missing values, and normalizing data to ensure accuracy and consistency across datasets.
3. Data Transformation: Performed transformations to prepare the data for analysis, including merging tables, reshaping data, and calculating new fields.

- **Data Modeling:**
1. Model Design: Created a well-structured data model that connected multiple tables with relationships (fact and dimension tables), ensuring efficient data querying.
2. Key Calculations: Developed calculated columns and measures to derive insights such as average delivery time, order trends, and satisfaction scores.

- **DAX Measures Creation:**

1. Complex Calculations: Utilized DAX (Data Analysis Expressions) to create measures for performance metrics like total rating count, active users, revenue, order counts, customer satisfaction etc.
2. Dynamic Reporting: Implemented DAX for time intelligence, comparisons (YoY, MoM), and other dynamic calculations to make the dashboard interactive and adaptable to different analysis perspectives.

- **Visualization Development:**

1. Interactive Dashboards: Designed a dashboard with clear, intuitive visuals such as bar charts, line graphs, KPIs, and heat maps to display key metrics.
2. User Experience: Focused on user-friendly navigation, including filters and slicers to enable dynamic exploration of data.
3. Storytelling with Data: Structured the visualizations to guide users through insights, highlighting key takeaways and trends.

- **Key Tools Used:**
1. Microsoft Power BI: For data modeling, DAX measures, and visualizations.
2. Excel: For preliminary data cleaning and manipulation.

## Data Modelling
It involves creating a structured and efficient schema to analyze the relationships and metrics across the various datasets.

![image](https://github.com/user-attachments/assets/d2903fa7-2956-4ec4-98af-46fccbc13f3d)

**Establish Relationships:**

- One-to-Many Relationships:
1. Users to Orders: One user can place many orders. (User ID in Orders table)
2. Food to Menu: One food item can appear in many menu categories. (Food ID in Menu table)
3. Restaurant to Orders: One restaurant can handle many orders. (Restaurant ID in Orders table)

- Many-to-Many Relationships:
1. Menu and Orders: Through Menu, multiple food items can be part of many orders.

## Dashboard

