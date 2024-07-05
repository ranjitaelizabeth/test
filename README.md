# test
###task1q-1.ipynb ;task1q-2,3,4 ;task2.ipynb are code files.

TASK 1:

1.Fixing Discontinuous Path in Latitude and Longitude Coordinates
•	Input Data:
Read the CSV file latitude_longitude_details.csv containing latitude and longitude pairs.
•	Identify Discontinuities:
Iterate through the coordinates to detect points where the distance between consecutive points exceeds a threshold, indicating a discontinuity.
•	Fixing Discontinuities:
Interpolate or adjust the coordinates to create a continuous path. This could involve methods like linear interpolation or smoothing techniques.
•	Save to CSV:
Save the corrected coordinates to a new CSV file, final_path_coordinates.csv.
•	Visualization:
Plot the original and corrected paths on a map using a plotting library like matplotlib or folium to show the before and after comparison

2.Calculate the KM distance and Save to database
•	Calculate KM values
•	Connect to the database 
•	Create the table and store the data
•	Executes query

3.Query points with terrain ‘road’ but not ‘civil station’

4.Exact boundary points for a given KM value


Task 2: 

1.Generate Points 25 Metres to the Left and Right: 
To generate points 25 meters to the left and right of given latitude and longitude coordinates, we can use the Haversine formula with geopy's distance module to calculate new points. Multi-threading or multi-processing can be employed to optimize the execution.
Concurrency: Using concurrent.futures.ThreadPoolExecutor allows us to process multiple coordinate transformations in parallel, significantly speeding up the computation compared to a single-threaded approach

2. Design a Data Structure for Moving Total:
To efficiently store and check if the total of any three successively added elements is equal to a given total, we can use a deque (double-ended queue) to maintain the latest three numbers and a set to store the sums of these triples.
Data Structure Choice: Using a deque is optimal because it allows efficient appending and popping from both ends, which is necessary to maintain a sliding window of the last three numbers. A set is used to store the sums, providing O(1) average time complexity for checking if a sum exists.

Python Modules Used:

numpy:For array operations
pandas: For reading and manipulating CSV data.
geopy: For geospatial calculations if needed.
matplotlib or folium: For plotting maps and visualizations.
psycopg2:For database connection (Postgresql )
Database :
Use PostgreSQL to store KM distances with terrain information. 
<img width="1470" alt="Screenshot 2024-07-05 at 10 23 17 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/57500faf-b735-4201-8c88-a7c11d7ca562">
<img width="1470" alt="Screenshot 2024-07-05 at 10 23 08 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/2f004aaa-64bd-4304-8b1a-d515d3cbf2f5">
<img width="1470" alt="Screenshot 2024-07-05 at 10 22 22 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/c132f994-0f4d-4145-b0a3-971a0b921660">
<img width="1470" alt="Screenshot 2024-07-05 at 10 20 45 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/d7acbee8-b974-4298-a6af-de2193cb162c">
<img width="1470" alt="Screenshot 2024-07-05 at 10 19 47 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/7913b086-c8da-4d1e-be26-06e00d25a63c">
<img width="1470" alt="Screenshot 2024-07-05 at 10 17 29 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/172cb434-ebe7-41da-8473-a99491e40f0b">
<img width="1470" alt="Screenshot 2024-07-05 at 10 17 22 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/4e06241a-53c9-410e-85de-d897f6b54695">

