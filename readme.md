# **IMPORTANT INSTRUCTIONS** (Please Read)

Since many of the `rou.xml` files (for testing and training) were too large to be committed to the Git repository, we were unable to push them to the Git repository (Git does not allow this). These files must be dynamically created by running the code. 

Please follow these steps:

1. **Run `create_route_file.ipynb`**:  
   This will regenerate a week's worth of training data using information from the database.  
   - This notebook creates all the SUMO `rou.xml` **training files**.

2. **Run `testing_route_file_creation.ipynb`**:  
   This notebook creates the **testing `rou.xml` file** for SUMO.

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
