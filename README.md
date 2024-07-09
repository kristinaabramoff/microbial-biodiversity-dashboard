# Belly Button Challenge

## Background
This project involved building an interactive dashboard to explore the Belly Button Biodiversity dataset, which catalogues microbes in human navels. The dataset reveals that a few microbial species (OTUs) were present in more than 70% of people, while others were relatively rare.

### Repository Setup
I created a repository named belly-button-challenge, cloned it, and copied the necessary files (index.html, samples.json, and the static folder) from the StarterCode folder. Changes were pushed to GitHub and the repository was deployed to GitHub Pages.

### Implementation
Data Loading
D3 library was used to read samples.json from the provided URL.

###  Bar Chart
A horizontal bar chart with a dropdown menu was created to display the top 10 OTUs found in an individual using:

sample_values for bar values
otu_ids for labels
otu_labels for hovertext

### Bubble Chart
A bubble chart was created to display each sample using:

otu_ids for x values and marker colors
sample_values for y values and marker size
otu_labels for text values

### Metadata Display
Sample metadata (demographic information) was displayed by looping through each key-value pair from the metadata JSON object and appending it to the #sample-metadata panel.

### Updating Plots
Plots and metadata update dynamically when a new sample is selected.

### Deployment
The app was successfully deployed to GitHub Pages. View the deployed app here.

### Files
index.html
samples.json
static/js/app.js
static/css/style.css
Skills and Programs Used
JavaScript: For building interactive charts and handling data.
D3.js: For data loading and manipulation.
Plotly.js: For creating bar and bubble charts.
HTML/CSS: For structuring and styling the web page.
Git & GitHub: For version control and deployment.
GitHub Pages: For hosting the deployed app.

## References
Hulcr, J. et al. (2012) A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable. Retrieved from: http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/Links to an external site.

