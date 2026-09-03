# 🌞 Accra Urban Solar Suitability & Investment Mapping Using Geospatial AI and Economic Modeling

Accra Solar Rooftop Suitability & Investment Intelligence. A geospatial AI pipeline and interactive decision-support tool for urban solar potential in central Accra, Ghana.

---

Final Preview

<p align="center">
  <img src="https://github.com/frankraDIUM/Building-Level-Solar-Suitability-Mapping-in-Urban-Ghana/blob/main/solar_new.gif" />
</p>
---



Dashboard Preview

<p align="center">
  <img src="https://github.com/frankraDIUM/Building-Level-Solar-Suitability-Mapping-in-Urban-Ghana/blob/main/Solar.gif" />
</p>
---

Solar Potential Density
<p align="center">
  <img src="https://github.com/frankraDIUM/Building-Level-Solar-Suitability-Mapping-in-Urban-Ghana/blob/main/Solar1.gif" />
</p>
---

Spatial Clusters
<p align="center">
  <img src="https://github.com/frankraDIUM/Building-Level-Solar-Suitability-Mapping-in-Urban-Ghana/blob/main/Solar2.gif" />
</p>
---

Top Investment Opportunities
<p align="center">
  <img src="https://github.com/frankraDIUM/Building-Level-Solar-Suitability-Mapping-in-Urban-Ghana/blob/main/Solar3.gif" />
</p>

---

Summary

  This project developed a scalable, end-to-end geospatial AI pipeline to assess rooftop solar potential across central Accra, Ghana. 
  
  The system integrates high-resolution building footprints, terrain-derived slope and aspect, NASA POWER solar irradiance data, 
  realistic economic modeling (including dynamic NPV and payback), shadow attenuation via building height proxies, 
  
  H3 hexagonal aggregation for scalability, and Getis-Ord Gi* hotspot analysis. 
  
  The result is an interactive Streamlit dashboard that supports multi-scale decision-making, from individual building investment to neighborhood-level policy planning.


Key outcomes:

  - Analyzed 632,195 buildings in the Greater Accra area.
  - Generated realistic solar potential estimates (mean ~12,408 kWh/year per building after shadow adjustment).
  - Produced dynamic ROI metrics with user-adjustable parameters (tariff, discount rate, self-consumption, cost per kW).
  - Identified spatial clusters of high solar investment potential using hotspot analysis.
  - Delivered a production-ready interactive dashboard with four distinct map views.


*1. Objectives*

Detect and characterize individual building rooftops using open building footprint datasets.
  - Assess technical solar suitability using slope, aspect, usable roof area, and shadow effects.
  - Estimate annual energy generation with performance losses and shadow attenuation.
  - Perform detailed economic analysis (payback period, NPV) with real-time sensitivity.
  - Aggregate results at hexagonal grid level for policy insights and performance.
  - Identify spatial investment hotspots and priority zones.
  - Provide an intuitive, interactive dashboard for stakeholders (households, SMEs, policymakers, investors).


*2. Key Results*

  - Total potential generation: ~6,000+ GWh/year (shadow-adjusted) across Accra.
  - Economic viability: Average simple payback ~7 years; many buildings show strong positive NPV.
  - High-potential buildings: ~81.5% have positive NPV under baseline assumptions.
  - Spatial insights: 44 hexagons identified as statistically significant hotspots (90%+ confidence).
  - Investment prioritization: Priority Score combines technical suitability, financial return, and spatial clustering for ranked decision support.

*3. Technical Implementation Highlights*

  - Scalability: Handles 632k+ buildings efficiently through vectorization, H3 aggregation, and caching.
  - Realism: Incorporates terrain constraints, shadow effects, degradation, O&M costs, and user-driven sensitivity analysis.
  - Multi-scale: Building-level detail + hexagonal policy view + hotspot detection.
  - User-centric: Interactive sliders, multiple synchronized views, export functionality, and clear legends.
  - Open & Reproducible: Relies on open datasets (Microsoft/Google buildings, Copernicus DEM, NASA POWER) and open-source tools (GeoPandas, Folium, H3, esda).
