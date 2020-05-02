+++
# A Demo section created with the Blank widget.
# Any elements can be added in the body: https://sourcethemes.com/academic/docs/writing-markdown-latex/
# Add more sections by duplicating this file and customizing to your requirements.

widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 1  # Order that this section will appear.

title = "Kazu konfirmadu total no foun iha Timor-Leste"
subtitle = "Timor-Leste iha kazu konfirmadu total 24: 22 iha Dili, no 2 iha Liquica."

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "1"

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.

  # Background color.
  # color = "navy"
  
  # Background gradient.
  # gradient_start = "DarkGreen"
  # gradient_end = "ForestGreen"
  
  # Background image.
  # image = "image.jpg"  # Name of image in `static/img/`.
  # image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.
  # image_size = "cover"  #  Options are `cover` (default), `contain`, or `actual` size.
  # image_position = "center"  # Options include `left`, `center` (default), or `right`.
  # image_parallax = true  # Use a fun parallax-like fixed background effect? true/false
  
  # Text color (true=light or false=dark).
  # text_color_light = true

[design.spacing]
  # Customize the section spacing. Order is top, right, bottom, left.
  padding = ["20px", "0", "20px", "0"]

[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""
+++

<script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
<script type="text/javascript">

  // Load the Visualization API and the corechart package.
  google.charts.load('current', {'packages':['corechart']});

  // Set a callback to run when the Google Visualization API is loaded.
  google.charts.setOnLoadCallback(drawChart);

  // Callback that creates and populates a data table,
  // instantiates the pie chart, passes in the data and
  // draws it.
  function drawChart() {
      var data = google.visualization.arrayToDataTable([
            ['Day', 'Kazu total', 'Kazu foun'],
            ["Mar 21, 2020",1,1],
            ["Mar 22, 2020",1,0],
            ["Mar 23, 2020",1,0],
            ["Mar 24, 2020",1,0],
            ["Mar 25, 2020",1,0],
            ["Mar 26, 2020",1,0],
            ["Mar 27, 2020",1,0],
            ["Mar 28, 2020",1,0],
            ["Mar 29, 2020",1,0],
            ["Mar 30, 2020",1,0],
            ["Mar 31, 2020",1,0],
            ["Apr 1, 2020",1,0],
            ["Apr 2, 2020",1,0],
            ["Apr 3, 2020",1,0],
            ["Apr 4, 2020",1,0],
            ["Apr 5, 2020",1,0],
            ["Apr 6, 2020",1,0],
            ["Apr 7, 2020",1,0],
            ["Apr 8, 2020",1,0],
            ["Apr 9, 2020",2,1],
            ["Apr 10, 2020",2,0],
            ["Apr 11, 2020",2,0],
            ["Apr 12, 2020",2,0],
            ["Apr 13, 2020",4,2],
            ["Apr 14, 2020",6,2],
            ["Apr 15, 2020",6,0],
            ["Apr 16, 2020",18,12],
            ["Apr 17, 2020",18,0],
            ["Apr 18, 2020",18,0],
            ["Apr 19, 2020",19,1],
            ["Apr 20, 2020",22,3],
            ["Apr 21, 2020",23,1],
            ["Apr 22, 2020",23,0],
            ["Apr 23, 2020",23,0],
            ["Apr 24, 2020",24,1],
            ["Apr 25, 2020",24,0],
            ["Apr 26, 2020",24,0],
            ["Apr 27, 2020",24,0],
            ["Apr 28, 2020",24,0],
            ["Apr 29, 2020",24,0],
            ["Apr 30, 2020",24,0],
            ["May 1, 2020",24,0],
      ]);

      var options = {
         title: '',
         curveType: 'none',
         legend: { position: 'bottom' },
         chartArea: {width: '95%', height: '80%', top: 5},
         hAxis: {showTextEvery: 10},
         annotations: { style: 'line' },
         focusTarget: 'category',
         height: 430,
         pointSize: 3,
         seriesType: 'bars',
         series: {0: {type: 'line'}}
      };

      var chart = new google.visualization.ComboChart(document.getElementById('cases-chart'));

      chart.draw(data, options);
  }
</script>
<div class="chart" id="cases-chart"></div>

