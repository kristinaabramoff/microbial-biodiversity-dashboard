# Microbial Biodiversity Interactive Dashboard

## Executive Summary
This project demonstrates proficiency in building interactive data visualizations using D3.js and Plotly, while also showcasing web deployment skills through GitHub Pages. The dashboard explores the Belly Button Biodiversity dataset, revealing insights into the microbial species colonizing human navels.

## Background
This project involves building an interactive dashboard to explore the Belly Button Biodiversity dataset, which catalogs the microbes found in human navels. The dataset shows that while a small number of microbial species (OTUs) were present in over 70% of individuals, many others were rare.

## Project Objective
The objective of this project is to create an interactive dashboard that visualizes data on microbial species found in belly button samples. Users can explore the top 10 OTUs found in each individual and view other data through dynamic bar and bubble charts, as well as sample metadata.

## Repository Setup
- A new repository named **microbial-biodiversity-dashboard** was created.
- The starter files (`index.html`, `samples.json`, and the `static` folder) were cloned and copied into the local repository.
- All changes were committed and pushed to GitHub, and the repository was deployed to **GitHub Pages**.
  - **View the deployed app**: [Microbial Biodiversity Dashboard](https://kristinaabramoff.github.io/belly-button-challenge/)

## Implementation

### Data Loading
The **D3** library was used to load the `samples.json` file from the provided URL.

### Bar Chart
A horizontal bar chart was developed to display the top 10 OTUs for a selected individual. It features:
- **Values**: `sample_values` representing the top 10 OTUs.
- **Labels**: `otu_ids` displayed as the bar chart labels.
- **Hovertext**: `otu_labels` shown when hovering over the bars for additional information.

### Bubble Chart
A bubble chart was developed to visualize all samples from the dataset. It includes:
- **X-axis**: `otu_ids` representing the OTU ID numbers.
- **Y-axis**: `sample_values` representing the sample values.
- **Marker size**: Proportional to `sample_values`.
- **Marker color**: Mapped to `otu_ids`.
- **Hovertext**: `otu_labels` providing more information about each OTU.

### Metadata Display
The demographic information of the selected individual is dynamically displayed. For each sample, the metadata (age, gender, location, etc.) is updated using a key-value pair loop and appended to the **#sample-metadata** panel.

### Plot Updates
Both the bar chart and bubble chart, along with the metadata display, update dynamically when a new sample is selected from the dropdown menu.

## Deployment
The dashboard was successfully deployed to GitHub Pages. The deployed app is accessible [here](https://kristinaabramoff.github.io/belly-button-challenge/).

## Files in this Repository
- `index.html`: The main HTML file for structuring the dashboard.
- `samples.json`: The dataset containing the belly button biodiversity data.
- `static/js/app.js`: Contains the JavaScript code for data loading, chart creation, and interactivity.
- `static/css/style.css`: CSS file for styling the dashboard.

## Technologies Used
- **Languages**: JavaScript (D3.js, Plotly.js), HTML, CSS
- **Tools**: Git, GitHub, GitHub Pages
- **Frameworks**: D3.js, Plotly.js

## References
Hulcr, J. et al. (2012) *A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable*. Retrieved from: [Rob Dunn Lab](http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/)

