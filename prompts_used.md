📑 **Prompts Used in Supply Chain Analytics Project**

While working on this project, I made use of AI-powered prompts in Quadratic to speed up tasks like data preparation, cleaning, and deriving business insights.
Below is a record of the main prompts I created and used.

🔹 **1. Date Table Creation**

Prompt Example:
"Generate a table containing all calendar dates starting from March 1, 2025, up to May 31, 2025."

🔹 **2. Exchange Rate Table**

Prompt Example:
"Prepare an exchange_rate table for the period March 1, 2025, to May 17, 2025. Use an exchange rate API request template and adjust the date parameter dynamically for each day in this range to collect INR conversion rates."

🔹 **3. Data Cleaning & Summary Table**

Prompt Example:
"Write Python code that does the following:

1.Import data from multiple sources:

    -Orders (fact_order_line)

    -Products (dim_products) – skip the first row and use the second as headers

    -Customers (dim_customers) – same formatting as above

    -Exchange rate data

2.Clean the datasets:

    -Convert IDs into proper numeric format

    -Remove whitespace and missing values

    -Change IDs into integers

    -Convert date columns to datetime type

3.Combine the datasets by:

    -Joining orders with products (via product_id)

    -Adding customer details (via customer_id)

    -Linking exchange rate data (via order_placement_date)

4.Perform calculations:

    For USD orders: price_USD * USD_INR_rate * order_qty

    For INR orders: price_INR * order_qty

5.Tidy the final output by:

    Dropping temporary columns (like raw prices, currency codes, rates)

    Keeping essential order info, IDs, dates, delivery status, and final amounts in INR."*

🔹 **4. Business KPI Development**

Prompt Example:
"Generate business KPIs such as:

    Total order lines

    Line fill rate

    Volume fill rate

    Total number of orders

    On-time delivery percentage

    In-full delivery percentage

    On-time in-full (OTIF) percentage"*

🔹 **5. Top Customers**

Prompt Example:
"List the top 5 customers by order value along with their OTIF %, IF %, and OT %. Include customer details like name, ID, and city in the output."


✨ **Note**: These prompts were designed by me inspired from codebasics for project execution. AI was used as an assistant to reduce repetitive tasks and speed up analysis, while the overall logic, workflow, and interpretation were done manually.
