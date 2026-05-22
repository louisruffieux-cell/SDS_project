#SDS-Project
---
##Introduction
This project analyses wildfires all around the world. With an API-query data is being downloaded from the NASA FIRMS website. Afterwards its beeing visualised with folium. 
The map includes three different layers that can be changed in the top right corner of the map:
    Layer 1: Choropleth layer, displays the density of widlfires(wildfires per 10'000km^2) from the last seven days
    Layer 2: Folium marker, displays the most recent wildfires that have been acitve the day before the code has been runs
    Layer 3: Heatmap layer, shows the developement of the wiildfires from the last seven days
After you ran the code the map lies in the Output folder. Open the html in your browser and have fun with the map

---
##Project structure

This is an overview of the projectstructure:
```text
├── data/                  # Folder of the Geodata 
├── notebooks/             # The project jupyternotebook(.ipynb)
├── environment.yml        # The conda environemnt (for the installation)
└── README.md              # This documentation
└── Outputs/               # The output of the map(html) and some plots
---
##Data needed

For the countries geometry download the ADM0(countrie) shapefile from the following website https://www.geoboundaries.org/globalDownloads.html

Put the downloaded folder in your data folder and dont change the name

##activate the environment

To replicate the software environment for this project, open your terminal, navigate into this project folder, and run the following commands

conda env create -f environment.yml

conda activate sds-project

aferwads open the jupyter notebook and use the sds-project environment