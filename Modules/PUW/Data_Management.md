---
layout: page
title: Tool 12 - Data Management and Visualization Support
permalink: /Data_Management_and_Visualization_Support/
parent: TOOLKIT - Water-Sensitive Infrastructure Development
grand_parent: Projects
nav_order: 13
---

![Banner]({{ site.baseurl }}/assets/Headers/Data management and Visualization Support.png){: style="width:100%; height:auto;" }


# Tool 12: Data Management and Visualization Support
_Authors: Juan Luis Ramirez Duval, Surendra Shiwakoti_

This tool provides an overview of using GeoNode for data management and visualization within the PUW framework. GeoNode is employed to facilitate the organization, sharing, and visualization of geospatial data to enhance cross-institutional collaboration, data-driven decision-making, and public engagement.

|        |  Data Management and Visualization Support      |
|:-------------|:------------------|
| **What?** | GeoNode is an open-source platform designed for managing geospatial data and providing tools for visualization and sharing. It supports creating interactive maps, managing geospatial layers, and fostering collaborative efforts in spatial data handling. Its features enable stakeholders to analyze, store, and disseminate urban water management data efficiently.|
| **Why? / Purpose** | GeoNode supports evidence-based urban planning and integrated water resource management by making data accessible and visually interpretable. It bridges communication gaps between stakeholders and promotes informed decision-making.  |
| **Field of Application** | GeoNode is applicable in various domains, including:<br>•	Cross-institutional data sharing<br>•	Urban water monitoring and management<br>•	Risk assessment and mitigation<br>•	Urban planning and infrastructure development|
| **End Users** |End users include municipalities and government agencies, researchers and academic institutions, urban planners, environmental consultants, and civil society organizations. |
| **Background** |GeoNode originated as a solution for geospatial data management and collaboration. With advances in technology, it has become a powerful tool for organizations aiming to make data-driven decisions in water and urban resource management. |
| **Description** | GeoNode facilitates:<br>•	**Data Management:** Uploading, categorizing, and storing geospatial data layers in centralized repositories.<br>•	**Visualization:** Creating user-friendly dashboards, interactive maps, and visual analytics.<br>•	**Collaboration:** Allowing multiple stakeholders to access, annotate, and share data in real-time.|
| **Strengths and Limitations** | **Strengths:** Enhances accessibility and sharing of geospatial data, supports real-time collaboration, enables powerful visualization through customizable maps, and is open-source with community support. <br> **Limitations:** Requires data literacy among users, depends on input data quality, and relies on stable IT infrastructure.|
| **Requirements  (Instruments Used)** | **Time:** Moderate <br> **Skills:** Comupter Proficiency, GIS knowledge.<br> **Equipment:** GeoNode Software, IT Infrastructure  <br> **Costs:** Low. |
| **Keywords** | GeoNode, Geospatial Data, Urban Water Management |

## Tool Manual

### _a. Tool Oveview_

This tool provides an overview of using GeoNode—an open-source platform for managing, visualizing, and sharing geospatial data—within the PUW framework. It outlines how GeoNode supports the organization and dissemination of urban water management data through interactive maps and geospatial layers, enabling cross-institutional collaboration, data-driven decision-making, and public engagement


### _b. Tool Usage Steps - HEC-RAS_

### 1. Accessing the Platform

To begin utilizing GeoNode, follow these steps to access the platform:
- **User Registration:** If you are a new user, navigate to the GeoNode homepage and select the 'Register' option. Fill in the required details, such as username, email, and password, to create     your account. Some GeoNode instances may require administrator approval for new accounts. Additionally, GeoNode supports integration with external authentication providers (e.g., LDAP, OAuth2), allowing users to log in using existing organizational credentials.
- **Logging In:** For existing users, click on the 'Login' button and enter your username and password. Upon successful authentication, you will be directed to your user dashboard.
- **User Dashboard:** The dashboard provides an overview of your activities, including uploaded datasets, created maps, and recent interactions. It also provides notifications about recent activities, such as comments on shared maps or datasets, facilitating better collaboration.
- **Navigation Menu:** GeoNode's interface includes a navigation menu with options such as 'Datasets,' 'Maps,' 'Documents,' and 'People.' These sections allow you to explore existing resources, create new ones, and interact with other users.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 75.png" alt="Figure_75" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 75: Creating account/logging into GeoNode.</figcaption>
</figure>
 


### 2. Uploading Data

GeoNode supports the upload of various geospatial data formats, including vector and raster data. To upload data:
- **Access the Upload Page:** Click on the 'Data' menu in the navigation bar and select 'Upload Layer' Alternatively, from the 'Layers' page, click the 'Upload Layers' button.
- Select Files: Use the 'Choose Files' button to select the geospatial files from your local system. Ensure that all necessary files for the dataset (e.g., .shp, .shx, .dbf, and .prj for shapefiles) are included. GeoNode supports additional formats like GeoTIFF, KML, and GeoJSON, offering flexibility in the types of data you can upload.
- **Set Permissions:** Before uploading, you can define who will have access to the data by setting permissions. This includes specifying who can view, download, edit, or manage the layer.
- **Metadata Standards:** GeoNode adheres to international metadata standards (e.g., ISO 19115), ensuring that your data is well-documented and easily discoverable by others. Providing comprehensive metadata enhances data interoperability and reuse.
- **Upload Files:** After selecting the files and setting permissions, click the 'Upload files' button to initiate the process. A progress bar will indicate the upload status. Once completed, you can view the uploaded layer's information to verify its correctness.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 76.png" alt="Figure_76" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 76. Data catalogue in GeoNode</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 77.png" alt="Figure_77" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 77. Data Uploading using GeoNode User Interface</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 78.png" alt="Figure_78" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 78. Upload datasets in GeoNode</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 79.png" alt="Figure_79" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 79. Upload datasets in GeoNode</figcaption>
</figure>

### 3. Managing Layers

After uploading, managing layers involves organizing, editing, and styling your geospatial data:
- **Layer Information:** Access the 'Layer Info' page to view metadata, including the layer's title, abstract, keywords, and spatial extent. Ensure that this information is accurate to facilitate data discovery and usage.
- **Editing Metadata:** If updates are needed, use the 'Edit' option to modify the layer's metadata. This includes updating descriptions, adding keywords, and setting the appropriate coordinate reference system (CRS).
- **Styling Layers:** GeoNode integrates with MapStore, offering advanced styling capabilities, including the creation of complex symbols and the application of data-driven styles. Customize the visual representation of your data by accessing the 'Style' tab. Define symbology, such as colors, line styles, and labels, to enhance the map's readability.
- **Attribute Management:** Through the attribute table, users can explore, edit, and analyze individual data attributes for each layer.
- **Setting Permissions:** Adjust permissions at any time to control access to your data. This is crucial for collaborative projects where different team members may require varying levels of access.
- **Deleting Layers:** If a layer is no longer needed, you can delete it by selecting the 'Delete' option. Be cautious, as this action is irreversible and will remove the data from the platform.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 80.png" alt="Figure_80" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 80. Dataset browser in GeoNode user interface</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 81.png" alt="Figure_81" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 81. Attribute viewer in GeoNode user interface</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 82.png" alt="Figure_82" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 82. Style customization in Geonode</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 83.png" alt="Figure_83" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 83. Editing style of geospatial data in GeoNode</figcaption>
</figure>


### 4. Creating Maps
GeoNode allows you to create interactive maps by combining multiple layers:

1. Initiate Map Creation: Navigate to the 'Maps' menu and select 'Create Map.' This opens the map viewer interface, where you can begin assembling your map.
2. Add Layers: Use the 'Add Layers' function to search for and select the datasets you wish to include. You can add multiple layers, adjusting their order to control visibility and overlap.
3. Configure Layer Settings: For each layer, you can adjust settings such as opacity, visibility, and display order. These controls help in creating a clear and informative map presentation.
4. Apply Styles: If you have predefined styles, apply them to the respective layers to ensure consistent symbology. This enhances the map's aesthetic and functional quality.
5. Add Annotations: Enhance your map by adding annotations, such as text labels, markers, and shapes, to highlight important features or provide additional context.
6. Save the Map: Once satisfied with the composition, save your map by providing a title, abstract, and relevant tags. This metadata facilitates easy retrieval and sharing of the map.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 84.png" alt="Figure_84" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 84. Creating a new map in GeoNode using the all resources or Maps tab</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 85.png" alt="Figure_85" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 85. Listing all existing maps in GeoNode</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 86.png" alt="Figure_86" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 86. Interactive visualization of dataset with map creation option in GeoNode</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 87.png" alt="Figure_87" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 87. Add multiple layers to the map from Datasets catalog in GeoNode</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 88.png" alt="Figure_88" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 88.  Interactive map with multiple geospatial datasets and basemaps in GeoNode</figcaption>
</figure>

### 5. Sharing and Collaboration

GeoNode emphasizes collaboration by enabling users to share resources and work together effectively:
- **Resource Sharing:** Share datasets, maps, and documents with specific users, groups, or the public. Generate shareable links or embed codes for external websites or platforms.
- **Groups and Communities:** Create user groups to collaborate on projects with specific stakeholders. Assign roles and permissions to group members for controlled data access.
- **Feedback and Comments:** Enable comments on layers and maps to gather input from collaborators. Use annotations to point out specific areas or issues within a dataset.
- **Notifications:** Set up alerts to notify you of updates, comments, or shared resources.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 89.png" alt="Figure_89" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 89. Configuration of sharing options for datasets, maps and documents</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 90.png" alt="Figure_90" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 90. High resolution map printing option in GeoNode</figcaption>
</figure>

### 6. Visualising Data
Visualization tools in GeoNode transform raw data into meaningful insights:
- **Dashboards:** Combine multiple visual elements, such as maps, charts, and tables, into a single dashboard. Use dashboards to present data summaries and analytics in an interactive format.
- **Filters and Queries:** Apply filters to focus on specific data subsets (e.g., date ranges, geographic areas). Use query tools to extract and display data matching custom criteria.
- **Heatmaps and Graphs:** Generate heatmaps to visualize density or intensity patterns. Create graphs, such as bar or pie charts, linked to geospatial features for statistical analysis.
- **Story Maps:** The storytelling feature combines maps with text, images, and multimedia. Present narratives about urban challenges, water resource management, or other themes.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 91.png" alt="Figure_91" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 91. Creating new Dashboard in GeoNode</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 92.png" alt="Figure_92" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 92. Creating new GeoStoriy in GeoNode</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 93.png" alt="Figure_93" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 93. Dual Map view in GeoNode Map Interface</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 94.png" alt="Figure_94" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 94. Available elements for designing GeoStories</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 95.png" alt="Figure_95" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 95. Designing GeoStory using multiple elements</figcaption>
</figure>

### 7. Collaborative Features

GeoNode fosters teamwork by providing robust collaborative tools:
- **Version Control and History:** Monitor changes to datasets and maps over time with built-in version history. Collaborators can view and revert to previous versions if necessary.
- **Real-Time Editing:** Enable simultaneous editing of datasets or maps by multiple users. Use locking mechanisms to prevent conflicts when two users modify the same feature.
- **Integration with External Tools:** Connect GeoNode with external GIS software like QGIS or ArcGIS for advanced editing. Export and import data seamlessly between platforms.
- **Discussion Forums:** Use integrated forums or comment threads for team discussions. Document decisions and feedback within the GeoNode environment.


<figure style="text-align: center;">
  <div style="display: flex; gap: 1rem; width: 100%;">
    <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 96A.png" style="width: 60%;" alt="Figure_96A">
    <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 96B.png" style="width: 40%;" alt="Figure_96B">
  </div>
  <figcaption>
    Figure 96. Browsing Geonode datasets in QGIS platform using Geonode plugin.
  </figcaption>
</figure>

## Further Reading

GeoNode Official Documentation: https://docs.geonode.org