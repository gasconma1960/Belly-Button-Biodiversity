# Belly-Button-Biodiversity
**Source:** Javascript, Plotly, D3 Libraries

**Image:** https://www.themarysue.com/wp-content/uploads/2011/01/bellybuttonbacteria-550x403.jpg

**Link to my webpage:** https://gasconma1960.github.io/Belly-Button-Biodiversity/

## Background
  Roza has a partially completed dashboard that she needs to finish. She has a completed panel for demographic information and now needs to visualize the bacterial data for each volunteer. Specifically, her volunteers should be able to identify the top 10 bacterial species in their belly buttons. That way, if Improbable Beef identifies a species as a candidate to manufacture synthetic beef, Roza's volunteers will be able to identify whether that species is found in their navel.


 ![image](https://user-images.githubusercontent.com/112348240/211173633-dba58987-ea65-4156-ac0f-5aa6b7799b5c.png)

## **Deliverable 1:** Create a Horizontal Bar Chart 
Using my knowledge of JavaScript, Plotly, and D3.js, create a horizontal bar chart to display the top 10 bacterial species (OTUs) when an individual’s ID is selected from the dropdown menu on the webpage. The horizontal bar chart will display the `sample_values` as the values, the `otu_ids` as the labels, and the `otu_labels` as the hover text for the bars on the chart.

My bar chart should look like the following image:

![image](https://user-images.githubusercontent.com/112348240/211173795-f83ba806-281e-4181-8859-2f07e995841c.png)

Add my starter code files to your GitHub pages (GitHub.io) folder. You will be editing the `charts.js` file for this deliverable. This file includes comments that indicate which instructions are for which deliverable. Use the instructions below to add code where indicated by the numbered-step comments in the starter code file. Follow the comments labeled **"Deliverable 1"** in the file to add your code.

In Steps 3-6, you’ll initialize variables that hold arrays for the sample that is selected from the dropdown menu on the webpage.

Make sure that you use `console.log()` to help debug any issues.

1. In Step 1, we’ve provided the code for the `buildCharts()`; function that contains the argument sample, which is the sample that is selected from the dropdown menu.

2. In Step 2, we’ve provided the code to retrieve the `samples.json` file using the `d3.json().then()` method.

3. In Step 3, create a variable that has the array for all the samples.

4. In Step 4, create a variable that will hold an array that contains all the data from the new sample that is chosen from the dropdown menu. To retrieve the data from the new sample, filter the variable created in Step 3 for the sample `id` that matches the new sample `id` chosen from the dropdown menu and passed into the `buildCharts()` function as the argument.

5. In Step 5, create a variable that holds the first sample in the array.
You can combine Steps 4 and 5 as one line of code, but make sure you use the correct variable name for Step 6 when retrieving the array data.

6. In Step 6, create variables that have arrays for otu_ids, otu_labels, and sample_values.

7. In Step 7, create the `yticks` for the bar chart.

In Steps 8-10, create the `trace` object, the layout, and `Plotly.newPlot()` function for the horizontal bar chart.

8. In Step 8, create the `trace` object for the bar chart, where the x values are the `sample_values` and the hover text for the bars are the `otu_labels` in descending order.

9. In Step 9, create the layout for the bar chart that includes a title.

10 In Step 10, use the `Plotly.newPlot()` function to plot the trace object with the layout.

After you have completed the coding requirements, your dashboard will look like this image when it loads for the first time:

![image](https://user-images.githubusercontent.com/112348240/211174045-5fb5c31e-ef30-460f-9a4b-ac4748c6ec9e.png)

## **Deliverable 2:** Create a Bubble Chart
Using your knowledge of JavaScript, Plotly, and D3.js, create a bubble chart that will display the following when an individual’s ID is selected from the dropdown menu webpage:

- The `otu_ids` as the x-axis values.

- The `sample_values` as the y-axis values.

- The `sample_values` as the marker size.

- The `otu_ids` as the marker colors.

- The `otu_labels` as the hover-text values.

Your bubble chart should look like the following image:
![image](https://user-images.githubusercontent.com/112348240/211174153-7c616b0b-176e-4b04-8f1c-0ffd0bf7cc55.png)





**Module 13 Challenge**

by Marisol Gascon Linarez
