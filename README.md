# MODULE 6 CHALLENGE : San Francisco Housing Analysis

In this challenge our job is to use our analysis, data visualization skills to find properties in the San Francisco market that are viable investment opportunities. In this challenge we are to calculate and plot the number of housing units per year, calculate and plot the average sale prices per square foot, compare those prices by neighborhoods with widgets, build an interactive neighborhood map, and provide analysis for the data. The data that we are starting from a csv file so we use the read_csv command, along with the pd command to import the census data and create a dataframe with it.

To calculate and plot the number of housing units per year we want to use the groupby function to group the data by year. When using the group by function we also have to aggregate the results, and to do this we are going to use the mean function. To plot our resuting dataframe we want to use the .hvplot and .bar function, and make sure to specify what variables we want the axes to correlate. 

To calculate the average sale prices per square foot we create a new dataframe like before, using the groupby function along with the mean aggregation. This time we only want to deal with the sale prices and gross rent columns so we use the drop function to filter out the housing units column. To plot our resulting dataframe we use the hvplot and line function to produce a line graph that visualizes the sale prices per square foot and the gross rent over the seven year period in the dataframe.

To compare the average sale prices by neighborhood we use widgets help create an interactive plot for each neighborhood. We would use the same syntax as before except inside the parentheses for the line function we would also include a groupby function and have it grouped by neighborhoods so there will be a widget on the side to specify what neighborhood we would like to view.

To build an interactive map of the neighborhoods we are going to have to read another csv file that has the respective coordinates for each of the neighborhoods, and we are going to specify that the neighborhood column is going to be the index column. We are then going to create another dataframe just like we did in the beginning of the challenge with using the groupby function and grouping the data by neighborhoods this time as well as taking the average of the results. We do this so that the index of this dataframe will be the same as the index of the dataframe with the coordinates. We want to combine the two dataframes by using the concat function to concatenate the two dataframe and its going to add the coordinates to our main dataframe that we have been working with prior. Some of the neighborhoods do not have coordinates listed and or some neigborhoods from the coordinates dataframe do not have housing information so to get rid of the NaN values we see we use the dropna function. To actually plot the map we use the hvplot and points function while specifying that we want the map displayed based on the coordinates and set the appropriate variables for the colors and sizes. Once that is done you can hover and use the other interactive features to see the gross rent and sale price per square foot for each neighborhood on the map. 


---

## Technologies

This project leverages python 3.7 with the following packages:

* [Pandas](https://github.com/google/pandas) - Pandas is a powerfull tool for data analysis and manipulation. Pandas provides a plethora of useful functions that make it easy to express, analyze, and manipulate data.

* [Hvplot](https://github.com/google/hvplot) - This Module provides a high-level potting API that allows for users to easily generate a wide array of plot types. HvPlot's main benefit is that it allows for very interactive visualizations.


---

## Installation Guide

Before running the application first install the following dependencies.

```
import pandas as pd
import hvplot.pandas
from pathlib import path


```

---

## Usage

To use the Financial Planning Tools file simply clone the repository and open the san_francisco_housing.ipynb file in Jupyter Notebook.

Upon opening the file you will have the option to run the whole note book and that will provide you with all of the calculations, evaluations, and visualizations for the valuations of crypto wallets and investment portfolios. Determining if members have enough to build an emergency fund into their financial plan, and forecasting of the cumulative returns of retirement portfolios.


This is where we used the json.dumps function to review the response data from the api call we used for BTC.![Screenshot 2022-08-03 193852](https://user-images.githubusercontent.com/107158380/182755890-ef8acb8d-ccfc-4d78-b0b7-1ef42b369ece.png)

This is where we used the json.dumps function to review the response data from the api call we used for ETH.![Screenshot 2022-08-03 193923](https://user-images.githubusercontent.com/107158380/182755928-f64a6925-1048-4cd6-9a41-faf81a6da32b.png)

This is where we displayed the dataframe of the investment portfolio after reorganizing and concatenating the two dataframes from each ticker.![Screenshot 2022-08-03 193950](https://user-images.githubusercontent.com/107158380/182756118-5b3adf38-b4f5-4a7e-abe5-05ff14898352.png)

This is where we displayed the dataframe of the list of the entire financial assets data, the crypto wallet and the investment portfolio.![Screenshot 2022-08-03 194116](https://user-images.githubusercontent.com/107158380/182756337-fbd04482-84cd-4e38-a546-a374fb74a3e7.png)

This is where we plotted a pie chart of that dataframe to help visualize the composition of the member's entire portfolio.![Screenshot 2022-08-03 194143](https://user-images.githubusercontent.com/107158380/182756453-b722f6c0-7376-4d17-95a7-73cef27d881c.png)

This is where we displayed the dataframe of the historical data/closing prices after reorganizing and concatenating the two dataframes from each ticker.![Screenshot 2022-08-03 194222](https://user-images.githubusercontent.com/107158380/182756714-165bb78f-5a8d-4f0c-abea-a4731aba7c68.png)

This is where we displayed the 30 year simulation dataframe after running our simulation. ![Screenshot 2022-08-03 194256](https://user-images.githubusercontent.com/107158380/182756958-709bf833-54ab-4e6e-80ae-34f73331eebe.png)

This is where we used the calc_cumulative_return() function to get the cumulative returns of each simulation. ![Screenshot 2022-08-03 194409](https://user-images.githubusercontent.com/107158380/182757167-86bebaee-9dc0-4e30-9e9f-8adf149d26ef.png)

This is where we displayed the simulated cumulative returns of the thirty year simulation with a line plot. ![Screenshot 2022-08-03 194438](https://user-images.githubusercontent.com/107158380/182757264-a18406b9-4e3d-4306-bd89-f5988ec05b07.png)

This is where we displayed the probability distribution of the thirty year simulation with a histogram.![Screenshot 2022-08-03 194502](https://user-images.githubusercontent.com/107158380/182757413-55a44ce2-f462-40fd-aff5-e638c773f34a.png)

This is where we displayed the summary statistics of the cumulative returns of the thirty year simulation.![Screenshot 2022-08-03 194523](https://user-images.githubusercontent.com/107158380/182757505-383ade7f-9385-482b-8088-180f1c0e868e.png)

This is where we displayed the 10 year simulation dataframe after running our simulation.![Screenshot 2022-08-03 194608](https://user-images.githubusercontent.com/107158380/182757570-495b1b48-53c0-43d0-8db1-81a1b8c9e462.png)

This is where we used the calc_cumulative_return() function to get the cumulative returns of each simulation.![Screenshot 2022-08-03 194629](https://user-images.githubusercontent.com/107158380/182757629-7d8fc93c-672e-4cfb-b7a0-ed993d6522af.png)

This is where we displayed the simulated cumulative returns of the ten year simulation with a line plot.![Screenshot 2022-08-03 194650](https://user-images.githubusercontent.com/107158380/182757672-79a781fa-e270-465d-9389-9d160f7fa307.png)

This is where we displayed the probability distribution of the ten year simulation with a histogram.![Screenshot 2022-08-03 194707](https://user-images.githubusercontent.com/107158380/182757756-91cbd4bc-f68e-47cf-8a9f-e384bbc3688a.png)

This is where we displayed the summary statistics of the cumulative returns of the ten year simulation.![Screenshot 2022-08-03 194730](https://user-images.githubusercontent.com/107158380/182757801-ccd4695f-b4ce-4b4b-bc9b-4b0fb0887bf6.png)


It is not that simple when trying to invest for retirement. TIME is the biggest factor when it comes to investing for someone's retirement. Weighting the porfolio more heavily to stocks has the potential for a higher reward, but that comes with the higher risks that are associated with that. The CI lower and upper for the 10 year majority stocks portfolio are much lower than that of the 30 year balanced portfolio. It really would not be reccomended to invest mostly instocks unless you are really young or trying to play catchup. What is really recommended for investing in someone's retirement is to invest as much as you can as soon as you can. Trying to weight your portfolio more heavily to stocks is not something you want to do if you want to retire in ten years, because it is way too risky and as seen from this example, you are pretty much not even able to retire after ten years in the best case scenario, and in the worst case scenario you are going to have to give up your plan of retirement.

---

## Contributors

Completed by Adam Cooke

---

## License

MIT

