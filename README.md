# Quick-Solar-Radiation-Analysis with Genetic Algorithm
This Grasshopper Script is used for analyzing the total solar radiation of curved building envelopes.
Note: This Grasshopper script was created with the following versions:
Rhinoceros 8
lbt_gh 1.8.0
python 3.10.10
RADIANCE 5.4a
Openstudio 3.9.0
energyplus 24.2.0

Step 1 Create a 3d model (Case study building envelope) in Rhinoceros or AutoCAD. If created in AutoCAD, import in Rhinoceros and set a case study Brep.
Step 2 In the Grasshopper interface, set-up the weather input. Use EPWMap GH component, Toggle True and ImportEPW components. Download Philippine EPW and import epw file from https://wwww.ladybug.tools/epwmap/. Use Skymatrix and AnalysisPeriod components. Set weather input numer slider from January to December with office hours from 8:00AM to 5:00PM.
Step 3 Set-up the solar radiation study. Use the components: Legend Parameters, Heatmap, Concatenate, Incident radiation, List Item, Color range. Set Legend Parameters to min 1.0, max 1000, customized panel (Solar incident radiation) under total of Incident radiation component, and panel (Combined Flux intensity) under results and Mass addition components.
Step 4 Set-up Genetic algorithm
