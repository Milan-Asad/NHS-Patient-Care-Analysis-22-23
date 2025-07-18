# NHS-Patient-Care-Analysis-22-23

## DESCRIPTION
A passion project analysing NHS Hospital Episode Statistics to evaluate overall patient care, including admissions and a 5-year forecase model built using Statsmodel.

## SUMMARY OF DATA
![image](https://github.com/user-attachments/assets/43ade539-70ce-45e8-b606-ee83da1349a9)

## ANALYSIS:

### FAE AND FCE BY YEAR:
Here we see both FAE and FCE slowly rising year by year, with a dip during 2020-21. The dip was due to the pandemic but it rebounded. What can we infer from this?
- An increasing FAE and FCE suggest that the NHS is treating more patients, possibly due to medical advancements and organisational expansion, such as hiring more staff.
- Elective admissions have generally risen, indicating improved capacity to treat patients.
- Emergency admissions have also increased at a steady rate, reflecting greater reliance on emergency care, which could suggest a growing strain on NHS services.
- The dip during the pandemic was due to treatment delays, likely creating a backlog that may have impacted admissions in subsequent years.

### MALE AND FEMALE FCE BY AGE (2022-23):
- Both male and female FCE drop from the ages 0-4 to 5-9. The high FCE at 0-4 is highly likely due to newborns and possibly unfortunate complications during this stage
- The lowest FCE count was at 10-14

## PATIENT JOURNEY
<img width="951" height="533" alt="image" src="https://github.com/user-attachments/assets/727fe424-6dfd-42ad-9fd8-a4a76174c403" />

### SUMMARY
- Hospitals often have the highest discharge days on Friday, possibly to free up beds for the weekend, as well as to provide closure as less staff are available on weekends
- In 2020–21, NHS critical care records dropped sharply, likely due to overwhelmed hospitals, altered care pathways, and pandemic-related disruptions in data reporting—not reduced demand. The decrease reflects service strain, not a decline in patient need.

## CASES BY ETHNICITY
<img width="1113" height="623" alt="image" src="https://github.com/user-attachments/assets/0772b791-8cc2-4763-8edc-cef49d86e923" />

### SUMMARY:
- Elective cases were at 52.7% whilst Emergency cases were at 37.27%, showing that the majority of hospital admissions were planned rather than urgent, suggesting effective access to scheduled care services.

## 5 YEAR FORECAST:
![Figure_1 (1)](https://github.com/user-attachments/assets/56292bfc-d01d-42d3-b434-5716429d12e0)

### STEPS TAKEN TO CREATE THE FORECAST MODEL:
- Load the dataset using pandas.
- Group the data and aggregate the FAE and FCE columns.
- Fit an ARIMA model for FCEs and FAEs with the order (0 to forecast the next 5 years.
- Define the forecast years starting from '2023-24' to '2027-28'
- Combine the historical data with the forecasted data for FCEs and FAEs.
- Create a list of years combining both historical and forecasted years.
- Plot the historical FCEs and FAEs as solid lines and the forecasted FCEs and FAEs as dashed lines.
- Format the y-axis to display values in millions.
- Set the plot title, labels for the x-axis and y-axis, and add a legend.
- Adjust the x-axis tick labels to display the years in 'YYYY-YY' format.
- Display the plot showing both historical and forecasted data.
