# Belly Button Biodiversity

![Bacteria by filterforge.com](Images/bacteria_by_filterforgedotcom.jpg)

In this practice, I will build an interactive dashboard to explore the [Belly Button Biodiversity DataSet](http://robdunnlab.com/projects/belly-button-biodiversity/).

## Step 1 - Plotly.js

Use Plotly.js to build interactive charts for my dashboard.

* Create a PIE chart that uses data from my samples route (`/samples/<sample>`) to display the top 10 samples.

  * Use `sample_values` as the values for the PIE chart

  * Use `otu_ids` as the labels for the pie chart

  * Use `otu_labels` as the hovertext for the chart

  ![PIE Chart](Images/pie_chart.png)

* Create a Bubble Chart that uses data from my samples route (`/samples/<sample>`) to display each sample.

  * Use `otu_ids` for the x values

  * Use `sample_values` for the y values

  * Use `sample_values` for the marker size

  * Use `otu_ids` for the marker colors

  * Use `otu_labels` for the text values

  ![Bubble Chart](Images/bubble_chart.png)

* Display the sample metadata from the route `/metadata/<sample>`

  * Display each key/value pair from the metadata JSON object somewhere on the page

* Update all of the plots any time that a new sample is selected.



![Example Dashboard Page](Images/dashboard_part1.png)
![Example Dashboard Page](Images/dashboard_part2.png)

## Step 2 - Heroku

Deploy my Flask app to Heroku.

see the website: https://sg-belly-button.herokuapp.com/

- - -

## Advanced Challenge Practice (Optional)

The following task is completely optional and is very advanced.

* Adapt the Gauge Chart from <https://plot.ly/javascript/gauge-charts/> to plot the Weekly Washing Frequency obtained from the route `/wfreq/<sample>`

* Need to modify the example gauge code to account for values ranging from 0 - 9.

* Update the chart whenever a new sample is selected

![Weekly Washing Frequency Gauge](Images/gauge.png)

- - -

## Flask API

Use Flask API starter code to serve the data needed for my plots.

* Test routes by visiting each one in the browser.

- - -

## Hints

* Don't forget to `pip install -r requirements.txt` before start the server.

* Use `console.log` inside of JavaScript code to see what the data looks like at each step.

* Refer to the [Plotly.js Documentation](https://plot.ly/javascript/) when building the plots.

- - -


