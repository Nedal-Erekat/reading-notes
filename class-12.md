# ANIMATED CHARTS
### A great way to get started with charts is with _`Chart.js`_

### Setting up The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script

## Drawing a line chart
#### To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart.Next, we need to write a script that will retrieve the context of the canvas

#### The great things about Chart.js are that it’s simple to use and really very flexible. Plus, once you’ve mastered the basics here, you’ll discover that there are tons of options

## Drawing a pie chart
#### Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element:

> `<canvas id="countries" width="600" height="400"></canvas>`
#### Next, we need to get the context and to instantiate the chart:

> `var countries= document.getElementById("countries").getContext("2d");`
> `new Chart(countries).Pie(pieData, pieOptions);`
#### You’ll notice that this time, we are going to supply some options to the chart.Next we need to create the data.

# EX:

> <!DOCTYPE html>
> <html lang="en">
>     <head>
>         <meta charset="utf-8" />
>         <title>Chart.js demo</title>
>         <!-- import plugin script -->
>         <script src='Chart.min.js'></script>
>     </head>
>     <body>
>         <!-- line chart canvas element -->
>         <canvas id="buyers" width="600" height="400"></canvas>
>         <!-- pie chart canvas element -->
>         <canvas id="countries" width="600" height="400"></canvas>
>         <!-- bar chart canvas element -->
>         <canvas id="income" width="600" height="400"></canvas>
>         <script>
>             // line chart data
>             var buyerData = {
>                 labels : ["January","February","March","April","May","June"],
>                 datasets : [
>                 {
>                     fillColor : "rgba(172,194,132,0.4)",
>                     strokeColor : "#ACC26D",
>                     pointColor : "#fff",
>                     pointStrokeColor : "#9DB86D",
>                     data : [203,156,99,251,305,247]
>                 }
>             ]
>             }
>             // get line chart canvas
>             var buyers = document.getElementById('buyers').getContext('2d');
>             // draw line chart
>             new Chart(buyers).Line(buyerData);
>             // pie chart data
>             var pieData = [
>                 {
>                     value: 20,
>                     color:"#878BB6"
>                 },
>                 {
>                     value : 40,
>                     color : "#4ACAB4"
>                 },
>                 {
>                     value : 10,
>                     color : "#FF8153"
>                 },
>                 {
>                     value : 30,
>                     color : "#FFEA88"
>                 }
>             ];
>             // pie chart options
>             var pieOptions = {
>                  segmentShowStroke : false,
>                  animateScale : true
>             }
>             // get pie chart canvas
>             var countries= document.getElementById("countries").getContext("2d");
>             // draw pie chart
>             new Chart(countries).Pie(pieData, pieOptions);
>             // bar chart data
>             var barData = {
>                 labels : ["January","February","March","April","May","June"],
>                 datasets : [
>                     {
>                         fillColor : "#48A497",
>                         strokeColor : "#48A4D1",
>                         data : [456,479,324,569,702,600]
>                     },
>                     {
>                         fillColor : "rgba(73,188,170,0.4)",
>                         strokeColor : "rgba(72,174,209,0.4)",
>                         data : [364,504,605,400,345,320]
>                     }
>                 ]
>             }
>             // get bar chart canvas
>             var income = document.getElementById("income").getContext("2d");
>             // draw bar chart
>             new Chart(income).Bar(barData);
>         </script>
>     </body>
> </html>