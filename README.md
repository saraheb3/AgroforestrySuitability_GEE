# US Midwest Agroforestry Suitability Mapping Code
Google Earth Engine code accompanying Midwest agroforestry suitability mapping paper, "Mapping the social-ecological suitability of agroforestry in the US Midwest"
Authors: Sarah E. Castle, Daniel C. Miller, Chloe B. Wardropper

# Overview 
All code is made publically accessible for use in Google Earth Engine. All the assets required to run this code are made public in Google Earth Engine.

This code maps agroforestry's suitability across the US Midwest using geospatial multi-criteria decision analysis. We mapped priority areas where agroforestry is expected to reduce the risk of environmental degradation, provide productive tree growth, and be socially and economically viable. This code allows readers to replicate our analysis. It also includes the code for the GUI creating the Google Earth Engine app that is our Agroforestry Suitability Decision Support Tool. 

Our study used suitability mapping to meet the need for improved knowledge of the potential suitability of agroforestry in the US Midwest. The Agroforestry Suitability Decision Support Tool was developed to assist program administrators in identifying areas that are most suitable for targeting agroforestry practices. Our interactive decision support tool allows users to select criteria that align with their priorities.

Agroforestry encompasses a set of practices where trees and shrubs are intentionally integrated into agricultural and animal systems, such as in alley cropping, riparian buffers, silvopasture, and windbreaks (USDA). As interest in agroforestry grows, practitioners, policymakers, and researchers need effective tools to identify regions where agroforestry practices can be most effectively targeted. Our  Agroforestry Suitability Maps and Decision Support Tool aim to guide stakeholders, such as researchers and practitioners, in identifying areas where resources for agroforestry expansion will likely have the greatest impact. 

The Agroforestry Suitability Decision Support Tool allows users to define criteria for modeling agroforestry suitability for different agroforestry practices across the US Midwest. The tool allows users to specify which criteria they would like to include in the model and how they weigh the relative importance of each criterion in decision-making. The Agroforestry Decision Support tool runs the user's analysis with their defined parameters in real time to generate customized results. Users may run the model for the entire 12-state Midwest region or specific states, counties, or watersheds. The tool is hosted through a Google Earth Engine app, which can be accessed directly through this link: https://agroforestrymap.projects.earthengine.app/view/agroforestry-suitability-tool 
User guide for Agroforestry Suitability Decision Support Tool: https://zenodo.org/records/14194395

## Repository Contents
- `gee_scripts/`: Scripts for running the suitability mapping model.
- `gee_app/`: Code for the GEE-based decision support tool.
- ...

## Getting Started
1. Sign up for a Google Earth Engine account: [GEE Sign-up Link](https://earthengine.google.com/).
2. Clone this repository:
   ```bash
   git clone https://github.com/sarahecastle3//AgroforestrySuitability_Published.git
   
# Details of Methodology:
To determine agroforestry suitability, we incorporated four key criteria: environmental priority areas, tree growth suitability, social feasibility, and economic viability. Each of these criteria can be weighed according to users’ goals (0-5). The environmental priority areas criterion generates a layer showing regions with the relative importance for addressing concerns over soil erosion from water, soil erosion from wind, water quality (ground and surface), and soil carbon sequestration; each of these sub-criteria can be weighed according to users’ goals in the advanced settings. The tree growth suitability criterion generates a layer showing how many of the selected tree species are at least minimally suitable to grow across the region, based on climate and soil conditions. We created binary tree suitability maps for nine tree species that can be considered in the tree growth suitability criterion: apple, black walnut, chestnut, eastern cottonwood, hazelnut, pecan, persimmon, sycamore, and white oak. The social feasibility indicator is a county-level indicator using NASS Census data that maps the relative feasibility of expanding agroforestry to the region based on current social conditions. The social feasibility criterion layer is generated using the rate of current conservation practices (e.g., conservation easements and CRP enrollment), the rate of rotational grazing, the rate of rented land, the rate of new/beginning farmers, and the number of people hired for agricultural labor. We recommend setting the weight of the social feasibility criterion to zero when running county- or watershed-level analyses. The economic viability criterion indicates regions where agroforestry is likely to be economically competitive to existing systems: areas that are more marginal for conventional agriculture are rated as more suitable for agroforestry; areas that are highly profitable in conventional systems are rated as less suitable for agroforestry. The indicator is generated by weighing the county-level net farm income by the SSURGO National Commodity Crop Productivity Index.   

# Citation: 
Castle, S.E., Miller, D.C., & Wardropper, C. (accepted, 2025). Mapping the social-ecological suitability of agroforestry in the US Midwest. Environmental Research Letters.
