
# Africa GDP Visualization

This project is an interactive web-based visualization of GDP per capita for African countries. It uses **D3.js** to render a choropleth map and a line chart, allowing users to explore GDP trends over time.

---

## **Features**

* **Interactive Map**:
  Visualizes GDP per capita for each African country for a selected year.

  * Hover over countries to see GDP values.
  * Click a country to display its GDP trend over time in the line chart.

* **Line Chart**:
  Displays the GDP trend of a selected country over multiple years.

  * Includes axes with appropriate scaling.
  * Tooltips show year and GDP for precise inspection.

* **Customizable Color Scales**:
  Users can select from multiple color scales to view the GDP intensity on the map:

  * `interpolateRdYlGn`
  * `interpolateViridis`
  * `interpolateBrBG`
  * `interpolateCool`
  * `interpolateTurbo`

* **Dynamic Legend**:
  A gradient legend automatically updates based on the selected year and color scale.

---

## **Project Structure**

```
/project-root
│
├── index.html         # Main HTML file containing SVG containers
├── script.js          # JavaScript file with D3.js code
├── style.css          # Optional CSS for styling tooltips and layout
└── data/
    ├── africa.geojson         # GeoJSON file for Africa's country borders
    └── africa_gdp_per_capita.csv  # CSV file with GDP data per country per year
```

---

## **How it Works**

1. **Load Data**

   * GeoJSON for Africa’s countries.
   * CSV with GDP per capita values by year.

2. **Draw Map**

   * Maps each country with color based on GDP value for the selected year.
   * Colors are scaled according to the selected color scale.
   * Hovering highlights the country and shows a tooltip with GDP info.

3. **Draw Line Chart**

   * Clicking a country on the map draws a line chart showing GDP trends over the years.
   * Interactive tooltips allow precise reading of year and GDP values.

4. **Update Map**

   * Users can change the year via an input box, updating both the map coloring and legend.
   * Users can select different color scales to visualize data differently.

---

## **Dependencies**

* [D3.js v6+](https://d3js.org/)
* Modern web browser (Chrome, Firefox, Edge)

---

## **Usage**

1. Open `index.html` in a web browser.
2. Select a year from the input box to update the map.
3. Hover over a country to view GDP.
4. Click a country to view its GDP trend over time.
5. Change the color scale from the dropdown menu for different visual perspectives.

---

## **Future Improvements**

* Add responsive design for mobile screens.
* Include more economic indicators like population or inflation.
* Animate transitions when changing years or selecting countries.
* Enhance tooltips with more detailed economic information.


