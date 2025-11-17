# MIST4610Group4Project2

Group Name:
15058 Group 4

Team Members:
1. Aadi Nag @aadinag-uga
2. Sam Greenspan @SamGreenspan1
3. Chase Lessing @chase-aquaz18
4. Sam Kooran @samuel4610
5. Nicholas Wilson @wilsonnj1

Description of dataset:
The dataset, which is named Monthly and Annual Energy Consumption by Sector, was published on data.gov by the US Energy Information Administration. The dataset is showing different statistics on the United States’ primary and total energy consumption by the end-use sector (residential, commercial, industrial, transportation) and the electric power sector from January 1973 to July 2025. There are 13 columns and 630 rows of data. The data in every column except the first is displayed in quadrillion BTU (British Thermal Unit). The first column, simply titled month, is the month and year. The data is taken monthly, starting in January 1973 and ending in July 2025. The second column is the total fossil fuel production. This is the total amount of energy produced from things like coal, natural gas, and crude oil. The next column is nuclear electric power production, the total amount of energy generated from nuclear power plants. The next column is total renewable energy production, the total energy produced from sources such as hydroelectric power plants, solar panels, wind farms, and biomass. The next column is the total primary energy production, which is the total amount of energy produced from primary sources (fossil fuels, nuclear energy, renewable energy). The next two columns are primary energy imports and primary energy exports, which are the total amount of primary sources such as fossil fuels and nuclear energy that was imported into the US and the total amount exported from the US to foreign countries. The next column, primary energy net imports, is the difference of imports and exports, with a positive number meaning that more energy was imported than exported. This is followed by primary energy stock change, which is the monthly change in the amount of energy held in storage such as crude oil, gas, nuclear energy, etc. Next is total fossil fuels consumption, the amount of fossil fuels used in the United States. This is followed by nuclear electric power consumption, the amount of energy consumed through nuclear energy sources. The next column is total renewable energy consumption, the amount of energy consumed through renewable energy sources. The last column is total primary energy consumption which is the combined total amount of energy consumed through primary sources such as fossil fuels, nuclear energy, and renewable energy.

Manipulations Applied to the Dataset:
Splitting the combined month-and-year column was necessary so we could look at years separately rather than months, since month-level detail wasn’t useful for this dataset. Separating the two allowed us to focus on changes over time by year and made the data easier to filter and compare.
We also converted the original month-year field from a text format into a proper date type in Tableau. This ensured the data could be sorted chronologically and allowed us to accurately visualize trends in energy consumption over time.
We also added meaningful names to the columns that originally had no labels. This helped make the dataset easier to understand, organize, and use effectively during analysis and visualization.

Analysis and Results:
To what extent does the amount of total renewable energy produced by the United States impact the amount of primary energy that gets imported?

<img width="986" height="645" alt="image" src="https://github.com/user-attachments/assets/9978748d-80a2-4e98-ad8f-6ac450e02c2f" />

This chart illustrates the relationship between primary energy imports and total renewable energy production within the United States. The fitted logarithmic trendline shows a slight positive association, indicating that as U.S. primary energy imports increase, renewable energy production tends to rise modestly. However, as shown by an R-squared value of only about 0.105, this relationship is weak. This means that imports explain only about 11% of the variation in renewable energy output. This could indicate that producing more renewable energy does not necessarily reduce the need for primary energy, or it may simply reflect that both imports and renewable production rise in response to higher overall energy demand. Although the p-value is highly significant which suggests the trend is statistically real, the wide dispersion of data points indicates that renewable energy production is influenced far more by other factors, like policy decisions, technological advances, resource availability, and general financial investment. Overall, as renewable energy production increases, primary energy imports tend to increase slightly, but this relationship is weak and accounts for only about 11% of the variation in imports.

<img width="972" height="567" alt="image" src="https://github.com/user-attachments/assets/d5c19817-002e-4d24-8feb-81dd73813dad" />

<img width="972" height="640" alt="image" src="https://github.com/user-attachments/assets/2150627f-6145-417b-889a-81d0fc397637" />

Which energy sources are the most or least predictable for future US energy consumption/production?

<img width="986" height="522" alt="image" src="https://github.com/user-attachments/assets/40c95a3b-66dd-4eed-bbb5-78d46f45f1a5" />

This chart shows the trends of energy production over time. Based on MAPE (Mean Absolute Percentage Error) as well as analysis of month-to-month trends, fossil fuels production would be the most predictable with nuclear and renewables as moderately predictable. Forecasts show a slight decline in nuclear electric production and a steady rise in renewable energy production, though both sources remain broadly stable over time. Fossil fuels production maintains a strong upwards trend and will likely continue to increase. 

This chart shows long-term trends in US energy production and evaluates how predictable each energy source is based on historical volatility, month-to-month stability, and Mean Absolute Percentage Error (MAPE). The analysis indicates that fossil fuels are the most predictable energy source, as their production follows a consistent upward trajectory with relatively low short-term fluctuation. Nuclear and renewable energy production are moderately predictable: nuclear output remains broadly stable but shows a slight long-term decline, while renewables display steady growth with more month-to-month variability due to factors such as technology deployment cycles, policy changes, and weather-related influences. Overall, fossil fuels maintain the strongest upward trend and the highest forecast reliability, whereas nuclear and renewables exhibit more moderate but still meaningful levels of predictability over time.


