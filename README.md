# Customer Performance Dashboard

This project uses Adventure Works DW sales data to analyze customer performance.

## Objectives:

The objective of this project is to make a Dashboard where it must achieve the following objectives.

- Calculate the **Average Age** of the customers.
- Determine the **Total Count** of the customers.
- Implement a **Dynamic Ranking System** to identify the top-performing customers.
- Analyze Revenue based on  **Customers With Children or Without Children**.
- Examine Revenue based on Customer's **Age Group**.
- **Categorize Customers** based on their total orders and purchases.
	- **VIP Customers** - Having Total Orders >= 2 and Total Purchases >= 100
	- **Loyal Customers** - Having Total Orders >=2
	- **Periodic Customers** - Others
- Examine Revenue based on **Customer Gender**.


## Implementation:
Here I will explain how the project was implemented with actual DAX codes. But before I am going to share the end result with additional feature of **Dark and Light Themes**

#### Dark Theme:

![Image](https://github.com/user-attachments/assets/22e701de-ea64-41e0-9b08-3a2cb81eb7d2)


#### Light Theme:

![Image](https://github.com/user-attachments/assets/494bd72b-f1e6-467a-8fe7-af292ce1feb6)

The above pictures clearly show the dashboard has achieved the objectives that were set before.

I will now share each part of the dashboard with its corresponding Measures and Columns created via DAX.

#### Part 1:

![Image](https://github.com/user-attachments/assets/c8dc7dfa-32d7-4036-9336-2fe078fb8591)

This Part of the dashboard is aligned with the project's first and the 2nd objectives.

Here I have created a new measure namely average age with the following DAX code and displayed it using a card.

![Image](https://github.com/user-attachments/assets/496acaa5-9d5d-428a-988f-86d35c363152)

The Total Customer is also calculated and displayed the same way as above with below DAX code.

![Image](https://github.com/user-attachments/assets/1f7b78ab-8a22-4f05-93df-46ca847c113a)

#### Part 2:
![Image](https://github.com/user-attachments/assets/900a35d1-7f2b-4902-8c68-929550359527)

Here I have implemented the third objective of the Project.

First, I have created a new parameter namely **Dynamic** via 
**Modeling tab --> New Parameter --> Numeric Range**
Then display it with a dropdown slicer.

Secondly, to display the selected number from the dropdown within the text under the header, I have used the following DAX code.
