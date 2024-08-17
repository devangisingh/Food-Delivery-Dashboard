# Food-Delivery-Dashboard

## Objective
To design and implement an interactive Power BI dashboard that provides actionable insights into food delivery performance by analyzing key metrics such as orders, customer satisfaction, customer demographics, overall sales, food category and order trends. The dashboard aims to improve operational efficiency, identify bottlenecks, and support strategic decision-making by offering clear, data-driven visualizations that enable stakeholders to optimize delivery processes and enhance overall customer experience.

## Dataset
[Link to Dataset](https://drive.google.com/file/d/1cUdM0zzJfAJscFK_mEDL7KWZ2lc0Wizl/view?usp=drive_link)

The dashboard utilizes five primary Excel datasets to provide a comprehensive analysis:
- **Food:**
1. Contains details about individual food items available with their category & id
2. Key Fields: Food ID, Food Name and Category.

- **Users:**
1. Includes information about the customers.
2.  Key Fields: User ID, Name, Age, Gender, Marital Status, Occupation and restuarant id.

- **Orders:**
1. Records of each food order placed by users.
2. Key Fields: Order Date, User ID, Restaurant ID, Quantity, Sales and Currency.

- **Restaurant:**
1. Details about the restaurants participating in the food delivery service.
2. Key Fields: Restaurant ID, Name, Location, Cuisine Type, Contact Information, and Ratings.

- **Menu:**
1. Contains information about the menu items offered by each restaurant.
2. Key Fields: Menu ID, Restaurant ID, Food ID, Menu Category, Price and Cuisine.

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

**Data Relationships:**
1. Food and Menu: The Menu dataset links food items to specific restaurants.
2. Users and Orders: Orders are associated with users to track order history and customer behavior.
3. Restaurants and Orders: Orders are linked to restaurants to analyze performance and delivery metrics.
4. Menu and Orders: Orders linked to Menu describes what users ordered cusisine available in Menu.
   
**Establish Relationships:**
- One-to-Many Relationships:
1. Users to Orders: One user can place many orders. (User ID in Orders table)
2. Food to Menu: One food item can appear in many menu categories. (Food ID in Menu table)
3. Restaurant to Orders: One restaurant can handle many orders. (Restaurant ID in Orders table)

- Many-to-Many Relationships:
1. Menu and Orders: Through Menu, multiple food items can be part of many orders.

## Dashboard
The Power BI dashboard provides a comprehensive analysis of food delivery operations by integrating data from five key datasets: Food, Users, Orders, Restaurant, and Menu. The dashboard is designed to offer actionable insights into customer behavior & demographics, order trends & count, restaurant performance and food categories, facilitating data-driven decision-making and operational improvements.

[Link to Dashboard](https://app.powerbi.com/links/_t-xAjuRbw?ctid=f7848cfc-1f86-4c9b-b1a1-a62dccc8be2a&pbi_source=linkShare)
1. **Sales and Revenue:** Displays total sales generated, order count, rating count, total sales by city, total sales by year and the contribution of food categories to the total sales.

![image](https://github.com/user-attachments/assets/006c1371-87ba-4e2b-9546-900a52b26b4a)

**Insights:**
- Total sales reached 987M in terms of amount and 2M in terms of quantity.
- 148k users actively participated and provided valuable feedback.
- The year 2018 saw the highest sales volume.
- Veg cuisines led with 122M in sales, closely followed by non-veg cuisines with 104M in sales.
- Tirupati recorded the highest sales, with Electronic City, Baner, and Raipur trailing behind.
- The total number of orders reached 150k.

2. **Customer Overview:** Displays user demographics and account information such as the number of active users, geographical distribution, and user growth/loss over time.

![image](https://github.com/user-attachments/assets/f124b4a8-9449-4ce5-8c22-9a55b521ae60)

**Insights:**
- Out of 100k users, 78k are active.
- Of the total users, 57.2% are male and 42.8% are female.
- 69.1% of users are married, with 3.1% preferring not to disclose their marital status.
- The majority of users are students (53.4k), followed by employees (30.4k).
- The largest group of users is aged 23.
- A total of 12k users were gained, while 33k users were lost.

3. **Geographical Insights:** Offers a visualization to analyze delivery operations geographically, showing concentration of orders by region.

![image](https://github.com/user-attachments/assets/37df5cf8-22f8-49c0-8af4-acc2b9f132c5)

**Insights:**
- A total of 822 cities were included.
- The overall number of orders reached 150k.
- Among all cities, Bikaner ranked highest in terms of orders, rating count, and active users.
- Tirupati registered the highest sales, amounting to 43M.

4. **Summary Overview:** Displays overall summary which includes Active Users, Gender, Age, Occupation, Marital Status, Year, Orders, Food Preferences & Total Sales by various City.

![image](https://github.com/user-attachments/assets/06ab3de8-0e02-4796-85ac-13f886a83e46)

## Interactivity and Usability:
- Dynamic Filters and Slicers: Users can filter the dashboard by date ranges, restaurants, food categories, customer segments, and geographical regions, allowing for customizable data views and personalized insights.
- Interactive Visuals: The dashboard employs a wide range of interactive visuals, such as bar charts, line graphs and key metrics cards, making it easy to explore data and uncover patterns.
- Drill-Down Functionality: Users can drill down into specific details, such as seeing individual order details, comparing restaurants, or analyzing customer order history for more granular insights.

## Business Impact:
- Strategic Planning: Provides management with the necessary insights to make informed decisions on restaurant partnerships, menu optimization, pricing strategies, and customer engagement tactics.
- Customer Retention: Supports the identification of high-value customers and trends in customer satisfaction, helping tailor loyalty programs and customer retention strategies.
