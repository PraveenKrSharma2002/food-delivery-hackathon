🍔 Food Delivery Data Analysis – Hackathon Project

This repository contains the complete solution for the **Food Delivery Data Analysis Hackathon, 
where multiple data sources were combined to create a single analysis-ready dataset and answer business questions.



📂 Datasets Used

The project uses **three different file formats**, simulating real-world systems:

1. orders.csv 
   - Transactional data  
   - Contains order details such as order_id, user_id, restaurant_id, order_date, and total_amount  

2. users.json  
   - User master data  
   - Contains user details such as user_id, name, city, and membership type (Gold / Regular)  

3. restaurants.sql  
   - Restaurant master data  
   - Contains restaurant details such as restaurant_id, restaurant_name, cuisine, and rating  

---
🔄 Data Processing Steps

Step 1: Load CSV Data
- Loaded `orders.csv` using Pandas

Step 2: Load JSON Data
- Loaded `users.json` using Pandas

Step 3: Load SQL Data
- Parsed `restaurants.sql` file and converted restaurant data into a Pandas DataFrame

Step 4: Merge the Data
- Performed LEFT JOINs to retain all orders:
  - `orders.user_id → users.user_id`
  - `orders.restaurant_id → restaurants.restaurant_id`

Step 5: Create Final Dataset
- Combined all datasets into a single dataset:
  - Order details  
  - User information  
  - Restaurant information  

- Exported the final dataset as:

final_food_delivery_dataset.csv


📌This final dataset is the only source of truth for all analysis and questions in the hackathon.



📊 Analysis Performed

Using the final dataset, the following analyses were carried out:

- Order trends over time  
- User behavior analysis  
- City-wise performance  
- Cuisine-wise performance  
- Membership impact (Gold vs Regular)  
- Revenue distribution and seasonality  
- Rating-based revenue analysis  

All MCQs, numerical questions, and insights are derived strictly from the final dataset.



🧪 Tools & Technologies

- Python  
- Pandas  
- Google Colab (for execution)  
- GitHub (for version control and submission)



📁 Repository Structure

├── food_delivery_data_analysis.ipynb
├── final_food_delivery_dataset.csv
├── README.md




🚀 How to Run the Notebook

1. Open the notebook in Google Colab or Jupyter Notebook
2. Upload the required input files:
   - orders.csv
   - users.json
   - restaurants.sql
3. Run the cells step by step
4. The final dataset will be generated automatically



✅ Conclusion

This project demonstrates a complete end-to-end data engineering and analysis workflow, including:
- Handling multiple data formats
- Applying correct join logic
- Creating a clean, analysis-ready dataset
- Deriving meaningful business insights

---

👤 Author

Praveen Kumar Sharma 

Data Analysis | Hackathon Submission
