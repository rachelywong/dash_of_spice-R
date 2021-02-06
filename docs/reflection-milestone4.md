# Milestone 4 Reflection

### Functionality 
The app allows users to rank features that are most important to them using six sliders for different metrics. These six sliders and their values then update both the world map, and the top ten country list. The map will update by color depending on metrics entered by the user in the sliders. Individual countries on the map can be clicked on and this, in turn, updates the dropdown menu and populates the line graph and the bar chart directly below. This line graph shows the yearly trends for selected countries and a selected feature of interest. At the same time, the bar chart compares the 2020 happiness scores for two or more countries, showing the happiness rank of each country when the user hovers over the bar. When only one country is selected on the map or in the map dropdown menu, the bar chart displays a trend in the happiness score for that country from 2015 to 2020. By default, when no country is selected the line graph and the bar chart show the global average happiness score.

### Improvements and Addressing Feedback
Based on the TA feedback for Milestones 2, 3, and 4 which were very helpful, we have improved the ranking algorithm, wisely connected the visual features of our dashboard, and adjusted the layout. As for the TA suggestion related to creating a stacked bar chart instead of the table, we have decided that keeping the top 10 countries table connected to the slider and the current bar chart connected to the map would be a better representation of the overall picture of happiness in different countries of the world. We adhere to the position not to overload the user with voluminous information.

Overall, we focused on simplifying our app to only the key components. We have created a map, two concise graphs, and a table with limited countries rather than 150+ countries as we had originally designed. We also limited our use of the historical data to the last year with the exception of the line graph and the bar chart (for one single country).

With respect to our peer feedback, we fully agree with the presented suggestions and recommendations and worked them out earlier in Milestone 3 and in the current version of Milestone 4 on R.

### R vs. Python
In Milestone 2, connecting our map to the line graph proved to be quite difficult. The two objects had to be placed in the same function and treated as one object. With milestone 3 however, R and ggplotly made the design far easier to implement. Every country selected is simply passed to the graph and handled separately. On top of this, plotly provides a better default map view than altair. The current version of the map allows for zooming and scrolling which was a limitation of our previous dashboard map. One downside of using Dash with R was that there didn't appear to be as much reference documentation as compared to Dash with Python. Another drawback is the fact that customizing the design and functionality of a dashtable with Python is more advanced than that with R. For instance, in Python an option is available to make the table non-clickable, while with R there was a trick. After weighing these positive and negative aspects of using R and Python, we chose R/ggplotly for Milestone 4.

### Unresolved Issues
Since we work on laptops from different manufacturers and use different operating systems and web browsers, we have noticed that the representation of the table frame and its header on our dashboard differs on diverse systems. For example, the current version of the table is displayed normally on Windows using Microsoft Edge, while on MacBook Pro 13″ using Google Chrome the table takes on an unpresentable view in full screen mode. Moreover, we should mention that we tried the app review in Heroku but it did not work.