# **IMPORTANT INSTRUCTIONS** (Please Read)

Since a lot of the rou.xml files (for testing and training) were too large to be committed to the git repo, we were not able to push them to the git repository (git did not allow to do so). Please run create_route_file.ipynb to regenerate a week's worth of training data 
using information from the database. Essentially, the file create_route_file.ipynb creates all the SUMO rou.xml TRAINING files.

Please follow these steps:

1. **Run `create_route_file.ipynb`**:  
   This will regenerate a week's worth of training data using information from the database.  
   - This notebook creates all the SUMO `rou.xml` **training files**.

2. The TESTING rou.xml file is titled: testing_routes_sumo.rou.xml (The 24-hour XML file is large, so it is shared via this onedrive link: https://utoronto-my.sharepoint.com/:u:/g/personal/t_pazhaidam_mail_utoronto_ca/EWf09oxxA9REjshyd4aNKhgBTMEh8O3lH7czN5KqdKcYJw?e=eeCvhT )
Please let us know if you have trouble accessing the large testing route file.

3. **SUMO RL Implementation**:  
   The actual SUMO RL implementation, as well as the training and testing code, can be found in:  
   - `sumo_environment_train_and_test.ipynb`

---

## Required Dependencies

### Python Libraries to Install:
To run the notebooks successfully, ensure the following Python packages are installed:

- **General Libraries**:  
  `numpy`, `pandas`, `matplotlib`, `logging`

- **Geospatial and Visualization Libraries**:  
  `geopandas`, `shapely`, `folium`, `plotly`

- **Reinforcement Learning**:  
  `gym`, `stable-baselines3`, `traci`

- **API and Web Requests**:  
  `requests`

### Additional Requirements:

- **SUMO (Simulation of Urban MObility)**:  
  SUMO is required for running the simulations. Follow the official SUMO installation guide to install it on your system:  
  [SUMO Installation Guide](https://sumo.dlr.de/docs/Installing/index.html)

---

### Additional Resources:

- The code used to **extract data, preprocess it, and populate the database** can be found in:
  - `traffic_dataset_extraction.ipynb`
