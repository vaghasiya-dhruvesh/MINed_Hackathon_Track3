# SmartRoute Optimizer

![Project Banner](https://via.placeholder.com/800x200?text=SmartRoute+Optimizer)

## Overview

**SmartRoute Optimizer** is an AI/ML-based solution for automated delivery route planning. Built for the **MINeD Hackathon** at Nirma University, our project tackles the challenge posed by **INTECH Creative Services**: efficiently plan delivery trips that optimize vehicle capacity, minimize total distance, and meet strict delivery timeslots.

Our solution leverages:
- **Google OR-Tools** for solving the Vehicle Routing Problem (VRP)
- **Python** libraries such as Pandas, NumPy, Geopy, and Haversine for data processing and distance calculation

## Team

- **Team Name:** ITWIZZARDS
- **Team Members:** (List your 4 members here)

## Problem Statement

The challenge required us to design an algorithm that automatically creates trips by grouping shipments while considering:
- **Vehicle Capacity:** Ensure each vehicle is used at least 50% of its shipment capacity.
- **Time Windows:** Ensure shipments are delivered within the specified delivery timeslots.
- **Distance Optimization:** Minimize the overall travel distance (using approximations like MST distance).
- **Vehicle Allocation:** Preferentially allocate priority vehicles (3W, 4W-EV) before regular vehicles.

For detailed problem description, refer to the [Problem Statement PDF](./ProblemStatement.pdf) (if included in your repository).

## Project Structure

Since our repository contains a single Python file, the code is designed to run on interactive platforms:
- **Jupyter Notebook**
- **Google Colab**
- **Kaggle Notebooks**

## Requirements

To run the project, you'll need:
- **Python 3.x**
- **Required Python packages:**  
  - `pandas`
  - `numpy`
  - `geopy`
  - `haversine`
  - `ortools`
  - `openpyxl`

You can install the necessary packages using pip:

```bash
pip install pandas numpy geopy haversine ortools openpyxl


How to Run the Project
Using Jupyter Notebook:
Clone the repository:
bash
Copy
Edit
git clone https://github.com/yourusername/SmartRouteOptimizer.git
cd SmartRouteOptimizer
Open the notebook:
bash
Copy
Edit
jupyter notebook
Open the provided Python file (or convert it into a notebook cell) and run the cells sequentially.
Using Google Colab:
Upload the Python file to your Google Drive.
Open Google Colab and create a new notebook.
Mount your Google Drive:
python
Copy
Edit
from google.colab import drive
drive.mount('/content/drive')
Navigate to the location of the Python file and run the cells.
Alternatively, you can copy-paste the code into a Colab notebook and run it.
Using Kaggle Notebooks:
Create a new Kaggle Notebook.
Upload the Python file as a data file or copy its content into a cell.
Install the necessary packages (Kaggle usually has many pre-installed).
Run the cells sequentially.
Project Flow
Data Preprocessing:

Parse shipment delivery timeslots into start and end times.
Compute the distance matrix using the haversine formula.
Normalize and prepare vehicle and shipment data.
Modeling & Optimization:

Use Google OR-Tools to solve the VRP.
Implement distance and time callback functions.
Apply capacity and time window constraints.
Set a termination condition (e.g., 4-minute time limit) to ensure timely results.
Output:

The code outputs a set of optimized routes along with vehicle assignments and validations for capacity, time, and distance.
Results & Future Work
Results:
Our solution successfully generates feasible routes and vehicle assignments under the given constraints within the allotted runtime.

Future Improvements:

Explore alternative search strategies to enhance solution optimality.
Integrate real-time data (e.g., traffic) for dynamic routing.
Enhance scalability for larger datasets.
Conclusion
The SmartRoute Optimizer is a promising solution that streamlines delivery route planning using advanced AI/ML techniques. It addresses key logistical challenges such as capacity utilization, time window adherence, and distance minimization, making it a valuable tool for companies aiming to reduce operational costs and improve customer satisfaction.

Feel free to reach out or submit an issue for any questions or suggestions.

Happy Routing!
Team ITWIZZARDS
MINeD Hackathon at Nirma University
