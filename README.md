In this project, I worked on analysing the sales data for a fictitious company named Tailwind Trader generating an insightful decision to take actionable data-driven decision.Below are some of the task that I performed to accomplish my project.

1) Using MS Excel, I obtain data from various sources and then cleaned, transformed, and load the data for further analysis.
   
  ![dataset](https://github.com/user-attachments/assets/408f5904-32bd-4b7d-a518-e96320c654e4)

2) Cleaning, transforming, and loading data in Power BI
   ![load dataset](https://github.com/user-attachments/assets/100924a3-b035-435f-92ba-4c4da2da0802)

3) Designing a data model and modeling data in Power BI.
   ![data model](https://github.com/user-attachments/assets/705d1b98-0260-412c-bf85-656ee08ded57)

4) Creating model calculations using DAX and optimizing model performance
   
   CalendarTable = 
      ADDCOLUMNS(
      CALENDAR(DATE(2020, 1, 1), DATE(2023, 12, 31)),
      "Year", YEAR([Date]),
      "Month Number", MONTH([Date]),
      "Month", FORMAT([Date], "MMMM"),
      "Quarter", QUARTER([Date]),
      "Weekday", WEEKDAY([Date]),
      "Day", DAY([Date])
   )

   Sales in USD = 
      ADDCOLUMNS(
      Sales,
      "Country Name", RELATED(Countries[Country]),
      "Exchange Rate", RELATED('Exchange Data'[Exchange Rate]),
      "Exchange Currency", RELATED('Exchange Data'[Exchange Currency]),
      "Gross Revenue USD", [Gross Revenue] * RELATED('Exchange Data'[Exchange Rate]),
      "Net Revenue USD", [Net Revenue] * RELATED('Exchange Data'[Exchange Rate]),
      "Total Tax USD", [Total Tax] * RELATED('Exchange Data'[Exchange Rate])
    )

6) Creating and enhancing dashboards and reports for usability, storytelling, and identifying patterns and trends.
   ![dashboard 1](https://github.com/user-attachments/assets/93a30d01-8250-44e9-b6f3-2950ae140234)

   ![dashboard 2](https://github.com/user-attachments/assets/bfa5d977-8108-4f0c-b47e-ee14d0063cac)

7) Configuring alerts.
   ![alert](https://github.com/user-attachments/assets/7cf9af53-068e-43f6-a038-b2b5f429f77d)

8) QnA
   
   ![QNA 2](https://github.com/user-attachments/assets/942cef0b-a260-452e-b149-56f06e100bdb)

   ![QNA 3](https://github.com/user-attachments/assets/679bf853-525e-4254-9264-74b8798970a0)





   
