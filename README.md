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
![image](https://user-images.githubusercontent.com/112348240/211175125-c19a4c0b-4014-40b1-bb32-2b1f508eb31d.png)

2. In Step 2, we’ve provided the code to retrieve the `samples.json` file using the `d3.json().then()` method.

3. In Step 3, create a variable that has the array for all the samples.

4. In Step 4, create a variable that will hold an array that contains all the data from the new sample that is chosen from the dropdown menu. To retrieve the data from the new sample, filter the variable created in Step 3 for the sample `id` that matches the new sample `id` chosen from the dropdown menu and passed into the `buildCharts()` function as the argument.

5. In Step 5, create a variable that holds the first sample in the array.
You can combine Steps 4 and 5 as one line of code, but make sure you use the correct variable name for Step 6 when retrieving the array data.

6. In Step 6, create variables that have arrays for otu_ids, otu_labels, and sample_values.

7. In Step 7, create the `yticks` for the bar chart.
![image](https://user-images.githubusercontent.com/112348240/211175142-9eaf6462-ae85-416c-a472-b54051de7426.png)


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

I will edit my `charts.js` file for **Deliverable 2.** Follow the comments labeled **"Deliverable 2"** in the file to add my code.

Use the variables that were created in **Deliverable 1** to populate the bubble chart. Then, use the instructions below to write the code for the `trace` object, the layout, and `Plotly.newPlot()` function to create the bubble chart.

1. To create the `trace` object for the bubble chart do the following:
    - Assign the `otu_ids`, `sample_values`, and `otu_labels` to the x, y, and text properties, respectively.
    - For the mode and marker properties, the mode is "markers" and the `marker` property is a dictionary that defines the `size`, `color`, and `colorscale` of the markers.

2. To create the layout for the bubble chart, add a title, a label for the x-axis, margins, and the `hovermode` property. The `hovermode` should show the text of the bubble on the chart when you hover near that bubble.

3. Lastly, use the given `Plotly.newPlot()` function to plot the `trace` object and layout.

After you have completed the coding requirements, your dashboard will look like the image below when it loads for the first time, with the bar chart you created in **Deliverable 1** and the bubble chart.

![image](https://user-images.githubusercontent.com/112348240/211174477-2f997b87-1f03-4b86-a750-c6e5edf75cd4.png)

## **Deliverable 3:** Create a Gauge Chart
Using my knowledge of JavaScript, Plotly, and D3.js, create a gauge chart that displays the weekly washing frequency's value, and display the value as a measure from 0-10 on the progress bar in the gauge chart when an individual ID is selected from the dropdown menu.

My gauge chart should look similar to the following image:

![image](https://user-images.githubusercontent.com/112348240/211174759-f1d926eb-9b9e-43ce-ad24-d7ec9b009da9.png)

I will edit your `charts.js` file for **Deliverable 3.** Follow the comments labeled "Deliverable 3" in the file to add my code.

1. In Step 1, create a variable that filters the metadata array for an object in the array whose id property matches the ID number from the dropdown menu that is passed into `buildCharts()` function as the argument.

2. In Step 2, create a variable that holds the first sample in the array created in Step 2.

3. In Step 3, create a variable that converts the washing frequency to a floating point number.

4. In Step 4, create the trace object for the gauge chart.

5. In Step 5, create the layout for the gauge chart making sure that it fits in the `<div></div>` tag for the gauge id.

6. In Step 6, use the `Plotly.newPlot()` function to plot the `trace` object and the layout.

![image](https://user-images.githubusercontent.com/112348240/211175166-969bf22c-76ac-4622-b0a2-2e767ed963ae.png)


After I have completed the coding requirements, my dashboard look like this image when it loads for the first time, with the bar chart you created in Deliverable 1, the bubble chart created in Deliverable 2, and the gauge chart:

![image](https://user-images.githubusercontent.com/112348240/211173633-dba58987-ea65-4156-ac0f-5aa6b7799b5c.png)

## **Deliverable 4:** Customize the Dashboard 
Use my knowledge of HTML and Bootstrap to customize the webpage for my dashboard.

1. Customize my dashboard with three of the following:
    - Add an image to the jumbotron.
    ![image](https://user-images.githubusercontent.com/112348240/211175026-a7cdb941-206e-4718-9bdd-bab67ef6c67c.png)

    - Add background color or a variety of compatible colors to the webpage.
    ![image](https://user-images.githubusercontent.com/112348240/211175039-5b426b58-d53c-4c92-83f8-06c0b700e0a1.png)

    - Use a custom font with contrast for the colors.
    ![image](https://user-images.githubusercontent.com/112348240/211175055-952468a0-c953-4764-b4e4-de28a2e0b60e.png)
    
    - Add more information about the project as a paragraph on the page.
    - Add information about what each graph visualizes, either under or next to each graph.
    - Make the webpage mobile-responsive.
    - Change the layout of the page.
    - Add a navigation bar that allows you to select the bar or bubble chart on the page.
2. When the dashboard is first opened in a browser, ID 940’s data should be displayed in the dashboard, and the three charts should be working according to their requirements.
3. When a sample is selected, the dashboard should display the data in the panel and all three charts according to their requirements.
![image](https://user-images.githubusercontent.com/112348240/211175088-e0725c0b-ad65-425d-b855-642fdf0526b8.png)


**Module 13 Challenge**

by Marisol Gascon Linarez
