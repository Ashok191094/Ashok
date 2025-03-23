# Coffee Quality Report

### Report Link : https://app.powerbi.com/links/YGV_yMSn7a?ctid=f6116aec-c576-4921-ab3d-c197702ebca0&pbi_source=linkShare

## Problem Statement

The objective of this project is to analyze and visualize data related to coffee quality using Power BI, aiming to uncover insights into factors that affect coffee quality ratings. The project focuses on leveraging Power BI's capabilities to create interactive visualizations and dashboards that facilitate exploration and understanding of the dataset.
Project Outcome: The main outcome of the project is a series of interactive visualization Reports and dashboard created in Power BI that provide insights into the factors influencing coffee quality ratings. Key findings such as correlations between different attributes and overall quality, and potential patterns among different coffee varieties, Processing Methods, Altitude or origins.


The primary goals of this project are:

1. To identify the key determinants of coffee quality as evaluated through sensory attributes such as aroma, flavor, and acidity.
2. To explore the correlation between processing methods, origin regions, and coffee quality scores.
3. To identify trends or patterns in defect occurrences and their impact on overall coffee quality.
4. To analyze how different variables interact to influence the Total Cup Points, an overall measure of coffee quality.

Data Overview of Coffee Quality Data from CQI

The Coffee Quality Data from CQI includes various features such as:

Sensory Evaluations: Aroma, Flavor, Aftertaste, Acidity, Body, Balance, Uniformity, Clean Cup, Sweetness.
Defects: Category One (visual defects) and Category Two (taste defects).
Processing Methods: Washed/Wet, Natural/Dry, Pulped Natural/Honey, etc.
Origin Information: Country of origin, harvest year, and coffee variety.

Defects:

Defects are undesirable qualities that can occur in coffee beans during processing or storage. Defects can be categorized into two categories: Category One and Category Two defects.

Category One defects are primary defects that can be perceived through visual inspection of the coffee beans. These defects include Black beans, sour beans, insect-damaged beans, fungus-damaged beans, etc.

Category Two defects are secondary defects that are more subtle and can only be detected through tasting. These defects include Over-fermentation, staleness, rancidness, chemical taste, etc.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : Cleaned the missing data using transformation options.
- Step 5 : Changed data types according to the values.
- Step 6 : Create new colums with Month and Year extraced from existing date column.
- Step 7 : Applied changes and loaded the data into power bi desktop.
- Step 8 : created new measures for the calculations.
- Step 9 : Following measures were created.
            Avg_cup_points,
            Avg_coffee_quality,
            Target coffee Quality,
            Total Defects.
- Step 10 : Created visualisations to understand the business objective goals.

In the data we found washed/wet and Natural Dry are contributing more to the data. To get the accurate results we have gone with the Average values instead of Sum of the values.

Page 1 of the report talks about the Global Coffee Quality and the different variable influence the total cup points.


![Image](https://github.com/user-attachments/assets/13376bd7-1480-41fe-83e3-cc13350677f0)

Average coffee quality is 7.68

Average cup points is 83.71

We observed that most grading is happening in the month of November.

Also observed that the coffee quality and cup points are in the downwards trend over the years.

We observed avg cup points affected by number of defects and variety. Also cup points affected by processing method.

Page 2 of the reports talks about the defect analysis.

![Image](https://github.com/user-attachments/assets/19c25819-74f6-4cc8-b66e-3560925ebb47)

We found total defect count 494 in entire data set.

We have two types of defects. category one and category two defects.

Category one defects are 28.

Category two defects are 466.

We observed Ethiopia country is producing more defects than the other countries with 51 total defects.

As we observed most of the grading is happening in the month of November. Defects are also correlated with the grading month as we have highest number of defects in the month of November with 79 defects.

We also observed that Caturra variety is having highest number of category two defects with 67 defects and SHG variety with highest number of category one defects with 5 defects.

Overall we observed Caturra variety is having highest number of defects with 67 category two defects and 4 category one defects.

Page 3 of the report talks about the coffee quality by process methods and country.

![Image](https://github.com/user-attachments/assets/f47a8184-4f12-4f71-a943-0c1385fef17c)

We have total 22 distinct countries and 11 processing methods.

From this report we observed that most countries are following washed/wet and Natural/Dry processing methods.

Overall 19 countires are using Washed/Wet method and 11 countries are following Natural/Dry method to produce the coffee.

Coffee quality in those countries are also above the average coffee quality.

Page 4 of the report talks about the coffee quality affected by sensory attributes.

![Image](https://github.com/user-attachments/assets/38b0c60e-321d-4f55-9e7e-185c84ca26dd)

We found Castillo and Red Bourbon are the two top quality and Acidity, Aroma and Flavour are the key sensory attributes that affect the coffee quality.

I have also added drill through option to navigate through the pages using process method.

