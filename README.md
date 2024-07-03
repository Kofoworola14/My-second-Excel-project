# My-second-Excel-project
The data of my second project was gotten from the playground of mavenanalytics, and it was analysed using excel. 
The data involves the sales of a resturant within the first three months of the year 2023 and shows the most and least ordered items from the resturant during the three months.
The data revealed the cuisine that made the most sales for the resturant and the day of the week with the most and least sales.
From the data, i was able to discover the total sales made by the resturant within the three months and the month with the largest sale.
https://1drv.ms/x/c/50e7327cecf2e7aa/Earn8ux8MucggFCTAAAAAAABc8n4iuQnMW_Ux9qNxPJx3w?e=3g9drT
# Steps taken during the analysis;
The dataset of this project is from ‘Maven Analytics’ located in the playground. I discovered that the sales data of a particular restaurant was collated from the first three months of 2023. I built this dashboard using Excel, because it is a widely used tool for data analysis and it’s fun, so why not?.
This is how the dashboard looks:
 <img width="513" alt="Kofs2" src="https://github.com/Kofoworola14/My-second-Excel-project/assets/168651782/9f4b63c1-d084-43f6-b789-03059e43167e">
As you can see from the picture, the dataset is from a restaurant. What does it contain? at the top we have 5 KPI’s (Key Performance Indicators) which list the most ordered item, the least ordered item, the most ordered cuisine, the most expensive item and the total sales made. Below them is a bar chart to show the top five ordered items (in which hamburger is obviously the most ordered item, the green color explains it), another bar chart to show the bottom five ordered items (in which chicken tacos is obviously the least ordered), a column chart to show the ten most expensive items in the restaurant. Then we have a line chart to show the trend of orders during the week, a pie chart to show how orders were made during the month (as we can see, the dataset information from the first three months of the year), another pie chart showing how orders were made from each category. There is another line chart showing the trend of how the items were ordered.
My favourite part of the dashboard is actually the slicers on the left side. We can use them to filter our data and make our dashboard interactive, as they are connected to all the pivot charts in the dashboard.
Excel is a very interesting tool and it’s a basic data analysis tool, there’s no need to be nervous about using it, it’s really fun from the start. It was really fun creating this dashboard, as it’s my second excel project, though I still learnt new things while creating it.
Before jumping into how to create the dashboard, I already have the xlsx file on my GitHub profile, you can download and go through it to see things before building your own. 
Step 1: Download the dataset from the playground and open the file.
I already provided the link to the dataset above, you can also google ‘Maven Analytics’ and search for Resturant Sales in the playground. Once it’s downloaded, open the file and take a look:
This is the menu item table:<img width="253" alt="rem" src="https://github.com/Kofoworola14/My-second-Excel-project/assets/168651782/9ffacb4a-6238-4a3e-b052-7d1133a01ee5"> 
This is the order details table:
<img width="287" alt="reo" src="https://github.com/Kofoworola14/My-second-Excel-project/assets/168651782/91047c5b-fab5-4da2-a337-db54d43fa369"> 
Well, there are two tables in the dataset, we have 4 columns and 32 rows in the first table, while the second has 5 columns and 12,234 rows. The columns are pretty explanatory but a bit tricky, as they both have a column in common, but it’s not really a big deal.
Step 2: Observe the data well.
This step is really crucial, especially when there are two tables involved. The order detail table is a fact table, as it contains numeric data, while the menu item table is the dimension table. Why do you think Excel was chosen for this dataset? Well it’s because this dataset is a quantitative data involving numbers and Excel is a spreadsheet tool. You can choose to use VLOOKUP to merge the tables together in a single table, but it’s really stressful. So, instead I launched the Power Query Editor, from the Data menu and I was able to clean, filter and transform the dataset into a meaningful one. 
First, you click on the Data menu on the screen, click on Get Data, then click on Launch Power Query Editor. The features of the Power Query Editor is similar to that of Power BI.
This is for menu items:<img width="810" alt="rem2" src="https://github.com/Kofoworola14/My-second-Excel-project/assets/168651782/f4517983-d5db-4e0a-af14-d7b7cd0b40d4"> 
This is for order details:<img width="809" alt="reo2" src="https://github.com/Kofoworola14/My-second-Excel-project/assets/168651782/45e1c652-bd4a-4774-a65b-110065eecd40"> 
This is what happens after launching, you can just try playing around by checking the column profile to check for the number of empty cells, number of unique and distinct cells and also make sure that the data type tallies with the components in the cell. Let’s go through the tables to confirm. After confirming, then click on the Close & Load icon by the upper left side to go back to the file page on Excel.
Next thing I did was extracting the day name from the order date in the orders table, so I can use it in the line chart later. So, I went to the data icon, clicked on get data and clicked on launch power query editor. In the power query, I went to the add column ribbon while placing the cursor on the order date column. From the options provided, I clicked on the date ribbon, which has options like year, quarter, day, age. Of course, I clicked on the day option then day of the week. Then again, go to the home ribbon and close& load.
That’s it for preparing our data, let’s move on.
Step 3: Pivot Tables and Charts.
In this step we will build the Pivot tables and charts to be used in the dashboard. We will create 7 charts which are:
1.	Two bar charts for the top and bottom five ordered items.
2.	One column chart for the highest spend orders.
3.	Two line charts for the order trend by day of the week and trend of order items.
4.	Two pie charts for the order items by month and category.
You can obviously choose different data and different charts to visualize, I only visualized based on the questions in the playground and also based on the data I find worthy.
To create each of the pivot tables from the data, click on any cell in the table, go to ‘Insert’, click Pivot table then click ‘From Data Model’ since the data was edited in power query.<img width="878" alt="pivot" src="https://github.com/Kofoworola14/My-second-Excel-project/assets/168651782/1d15cea0-af26-49ef-b3d4-e40fb2c8ccfe">
You will be asked to select a location, then this appears:<img width="957" alt="pivot2" src="https://github.com/Kofoworola14/My-second-Excel-project/assets/168651782/83683b4b-a095-4b87-87b8-e99ffe669e9f"> 
To create each pivot table, drag any option of your choice from either the menu items or order details into the ‘values’ or ‘rows’ box. Next is to create the chart. Click on any cell from the pivot table and click on Pivot Chart on the right. In the pivot chart, you can click on any chart of your choice depending on the data you are to visualize.
Step 4: Building the Dashboard!
You can decide to use an online dashboard or create a dashboard on Excel. I mostly create my dashboards on Excel and trust me it’s so much fun.
First of all, I remove the gridlines on the excel workbook, by clicking on page layout and unticking the view box under gridline. It is made into a blank page like this:
<img width="943" alt="grid2" src="https://github.com/Kofoworola14/My-second-Excel-project/assets/168651782/032d52dc-532e-4c40-93b2-59c3a06d6e95"> 
After which you cut and paste your charts onto the dashboard. It is very important that you create your slicers from the pivot charts so the slicers created will be in connection with the pivot charts. Click on a pivot chart, then click on Pivot Chart Analyze, then Insert Slicer and tick the slicers you want to create.
<img width="954" alt="slicer" src="https://github.com/Kofoworola14/My-second-Excel-project/assets/168651782/7acf1a17-ce5b-4157-9002-e8d37a291851">
Then you report connections, so the slicers will interact with the charts. Then you can edit your dashboard and slicer into any colour of your choice.
Oops, I just realized I forgot to explain how to make the metrices or KPIs on top. Click on Insert > Text > Text box. Click inside the text box so it shows the typing cursor, then go to the formular box and type an ‘=’ sign, then go to the cell that has the value or name you want then press Enter. This links the text box to the cell.
Thanks for coming this far   !!!!!!!.
