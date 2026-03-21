# NYC Flooding: Who Gets Hurt the Most?

Welcome to the **FSHRI-Median Household Income** interactive dashboard! Its pupose is to show the median household income and the Flood Susceptibility to Harm and Recovery Index (FSHRI) in New York City. 

The tabs on the left will take you to different sections of the dashboard:
- **Home**: This page, with the interactive map experience
- **Charts**: A few additional visualizations of the dataset
- **About**: In-depth definitions of FSHRI and median household income, how they were calculated, and the sources of the data
- **Inspirations**: The artist that inspired this 3D map experience, Herwig Scherabon

<br>

## The Map
<br>

<style>
  .my-table {
    width: 100%;
    border-collapse: collapse; /* */
    margin: 25px 0;
    font-size: 0.9em;
    font-family: serif;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
  }
  .my-table th, .my-table td {
    border: 1px solid #dddddd; /* */
    padding: 12px 15px; /* */
    text-align: left;
  }
</style>

<table class="my-table">
<caption><b>Feature Descriptions and Legend</b></caption>
<tr>
<th>Feature</th>
<th>Description</th>
<th>Representation</th>
</tr>
<tr>
<td><b>Flood Susceptibility to Harm and Recovery Index (FSHRI)</b></td>
<td>Measure of a neighborhood's vulnerability to flooding events. Includes factors like population demographics, socioeconomic vulnerability, and recovery capacity.</td>
<td><b>Color</b>: The darkest blues are the most susceptible to harm from flooding, while the lightest are the least vulnerable.</td>
</tr>
<tr>
<td><b>Median Household Income</b></td>
<td>Median household income in past 12 months (inflation-adjusted to the last of the past 5 years) </td>
<td><b>Height</b>: The taller the neighborhood, the higher the median household income.</td>
</tr>
</table>

<br>
Search your neighborhood or click on the census tract to see your area's Flood Susceptibility to Harm and Recovery Index!

```js
const mapUrl = await FileAttachment("./map.html").url();
display(html`<iframe src="${mapUrl}" width="900px" height="500px" allowfullscreen="true" style="border: 1px solid #ccc; border-radius: 8px; margin-top: 20px;"></iframe>`);
```
<small>Tip: Use the scroll wheel to zoom in and out of the map. Click and drag to move the map. Hold Ctrl + Click and drag to rotate the map.</small>

<br>
<br>

<small>This documentation is written in Markdown and powered by [Observable Framework](https://observablehq.com/framework/).</small>