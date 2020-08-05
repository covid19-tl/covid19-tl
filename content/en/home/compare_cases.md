+++
widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 3  # Order that this section will appear.

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

## Confirmed cases per municipality


<script type="text/javascript">
  google.charts.load('current', {
    'packages':['geochart'],
    // Note: you will need to get a mapsApiKey for your project.
    // See: https://developers.google.com/chart/interactive/docs/basic_load_libs#load-settings
    'mapsApiKey': 'AIzaSyD-9tSrke72PouQMnMX-a7eZSW0jkFMBWY'
  });
  google.charts.setOnLoadCallback(drawRegionsMap);

  function drawRegionsMap() {
    var data = google.visualization.arrayToDataTable([
        ['Municipiu', 'Confirmed cases'],
        ['Aileu', 0],
        ['Ainaro', 0],
        ['Baucau', 0],
        ['Bobonaro', 0],
        ['Cova', 0],
        ['Dili', 23],
        ['Ermera', 0],
        ['Lautem', 0],
        ['Liquiça', 2],
        ['Manatuto', 0],
        ['Manufahi', 0],
        ['Oecussi', 0],
        ['Viqueque', 0],
    ]);

    var options = {
        region: 'TL',
        displayMode: 'regions',
        resolution: 'provinces',
        chartArea: {width: '95%', height: '80%', top: 5},
        colorAxis: {colors: ['red']}
    };

    var chart = new google.visualization.GeoChart(document.getElementById('municipality-map'));

    chart.draw(data, options);
  }
</script>

<div id="municipality-map"></div>
