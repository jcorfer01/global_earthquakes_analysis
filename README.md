# Analysing global earthquakes from the past 7 days
The goal of this project is to analyze real-time earthquake data streaming and gain insights into earthquake distribution across multiple factors. For this purpose, I am receiving streaming data through the notebook "DataEarthquake.ipynb", sourced from the [USGS](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php) public API, which provides earthquake data for the past 7 days on a global scale every 60 seconds.
<br><br>
As part of the analysis, I generate various visualizations that highlight the distribution of earthquakes across three key factors: location, magnitude, and time. These graphs aim to provide a deeper understanding of earthquake patterns and trends, offering a comprehensive overview of seismic activities worldwide.
<br><br>
To finish the analysis of the data received, I have included some statistical values of the earthquake's magnitudes such as: mean, median, standar deviation and variance. These metrics help quantify the overall characteristics and variability of seismic activity during the analyzed time frame. By examining these statistical values, we gain a clearer understanding of the typical magnitude of earthquakes, the spread of the data, and the occurrence of extreme values. This final step adds a quantitative perspective to the visualizations, providing a well-rounded analysis of the earthquakes data.
<br><br>
## Datasets Description:
Inside the USGS website there is a [Event Terms Documentation](https://earthquake.usgs.gov/data/comcat/data-eventterms.php#mag) with the data type, typical values and description for each element of the JSON file.
<br><br>
Here I include each field used in the analysis with a brief description taken from the official documentation:
<br>
<ul>
  <li>id: A (generally) two-character network identifier with a (generally) eight-character network-assigned code.</li>
  <li>properties
    <ul>
        <li>mag: The magnitude for the earthquake.</li>
        <li>place: Textual description of named geographic region near to the event. This may be a city name, or a Flinn-Engdahl Region name.</li>
        <li>time: Time when the event occurred. Times are reported in milliseconds since the epoch ( 1970-01-01T00:00:00.000Z), and do not include leap seconds. Inside the data ingest, the date is formatted for readability.</li>
        <li>updated: Time when the event was most recently updated. Times are reported in milliseconds since the epoch.</li>
    </ul>
  </li>
  <li>coordinates
    <ul>
        <li>longitude: Decimal degrees longitude. Negative values for western longitudes.</li>
        <li>latitude: Decimal degrees latitude. Negative values for southern latitudes.</li>
        <li>depth: Depth of the event in kilometers.</li>
    </ul>
  </li>
</ul>
