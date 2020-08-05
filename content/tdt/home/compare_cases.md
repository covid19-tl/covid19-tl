+++
widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 4  # Order that this section will appear.

[design]
  columns = "1"

[design.spacing]
  # Customize the section spacing. Order is top, right, bottom, left.
  padding = ["20px", "0", "20px", "0"]

[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""
+++

## Kazu konfirmadu iha kada municipiu


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
        ['Municipiu', 'Kazu konfirmadu'],
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
