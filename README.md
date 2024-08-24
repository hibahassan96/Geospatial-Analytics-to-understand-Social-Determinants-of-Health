# Geospatial-Analytics-to-understand-Social-Determinants-of-Health

All related project data and files can be accessed [here](https://drive.google.com/drive/folders/1PfdQ9qTtDnq0E_FhmBpQ4XDntJsdf6GL?usp=sharing)

## Project Motivation
The project aimed to analyze Social Determinants of Health (SDOH) within Allegheny County, with a specific focus on children and youth. By leveraging geospatial analytics and GIS tools, we sought to understand how various environmental and social factors, such as air quality, recreational spaces, and access to nutritious food, impact health outcomes. The goal was to identify health disparities and recommend actionable interventions for government agencies and nonprofits to improve the well-being of communities in the county.

## Methodology
The analysis was structured into three primary components:

### 1. **Air Quality and Respiratory Conditions**
   - **Data Sources**: UPMC Emergency Department Visits data, Allegheny County Air Quality Index, and 2010 Census Tracts.
   - **Process**: 
     - Imported datasets into ArcGIS, joined with city tract data using GEOID.
     - Mapped respiratory-related ER visits and air quality data using graduated colors and the Pairwise Buffer tool to define areas of influence.
   - **Tools Used**: ArcGIS, Pairwise Buffer, XY coordinates mapping.
![image](https://github.com/user-attachments/assets/3bb88244-aa0e-4c1f-a9a7-009fb14f185b)


### 2. **Obesity Rates and Influencing Factors**
   - **Data Sources**: Obesity rates (2006-2010), Fast Food Establishments, City Parks, Pools, Playgrounds, and 2010 Census Tracts.
   - **Process**:
     - Focused analysis on Pittsburgh's census tracts.
     - Utilized the 'Select by Location' tool for targeting relevant tracts.
     - Created choropleth maps to visualize obesity rates and employed spatial join for counting relevant facilities per census tract.
     - Performed linear regression analysis to assess correlations.
   - **Tools Used**: ArcGIS, Spatial Join, Choropleth mapping, Linear Regression.
![image](https://github.com/user-attachments/assets/bf118890-8eff-4495-bdf7-4bab6442098b)

### 3. **Health Index Creation**
   - **Data Sources**: Pittsburgh Police Arrest Data, Pediatric Emergency Department Visits, Obesity Rates, Poor Housing Conditions, and 2010 Census Tracts.
   - **Process**:
     - Created choropleth maps for various health indicators.
     - Computed Z-values for selected variables and constructed a Health Index.
     - Generated a choropleth map to visualize disparities.
   - **Tools Used**: ArcGIS, Calculate Field Tool, Model Builder for Health Index computation.
![image](https://github.com/user-attachments/assets/162af08a-f2c0-4ad6-a69e-9383ff80b4cd)

## Results
### **Air Quality and Respiratory Conditions**
- Key neighborhoods with poor air quality and high respiratory ER visits include Downtown, Lawrenceville, and Oakland. Poor air quality was identified as a contributing factor, particularly in areas with dense commercial activity and proximity to highways.

### **Obesity Rates and Influencing Factors**
- High obesity rates were observed in Downtown, North Shore, and Homewood. Although a slight correlation was found between obesity and fast-food presence or lack of sports facilities, the relationship was weak, suggesting other unmeasured variables may play a significant role.

### **Health Index and Community Spaces**
- The Health Index highlighted Northshore, Hill District, Homewood, Glen Hazel, and Garfield as areas with significant health disparities. These neighborhoods require targeted interventions, such as the establishment of community centers, to address underlying SDOH issues and improve health outcomes.

## Recommendations
- Implement community health initiatives focusing on improving air quality and providing better access to recreational spaces in identified high-risk areas.
- Develop policies to regulate the density of fast food establishments in vulnerable neighborhoods.
- Use the Health Index as a guide to allocate resources and plan new community health centers in the most affected regions, particularly in the Garfield neighborhood.
