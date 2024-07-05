EXPLANATIONS:

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
<img width="1470" alt="Screenshot 2024-07-05 at 10 23 17 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/8c574a2e-0e4b-472b-871b-269e7aeb13fa">
<img width="1470" alt="Screenshot 2024-07-05 at 10 23 08 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/9b215ed0-0598-48ba-8ec5-a56c6c2da70e">
<img width="1470" alt="Screenshot 2024-07-05 at 10 22 22 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/0c81a337-5676-4505-b89e-6e8b234d08f1">
<img width="1470" alt="Screenshot 2024-07-05 at 10 20 45 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/b9273e00-be4c-4f0c-81fb-77a16b4c436c">
<img width="1470" alt="Screenshot 2024-07-05 at 10 19 47 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/20a51d7b-9728-4a50-9c91-4df8935d5e59">
<img width="1470" alt="Screenshot 2024-07-05 at 10 17 29 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/0dfcd56b-cda4-49eb-9279-4fbecdb0dfbe">
<img width="1470" alt="Screenshot 2024-07-05 at 10 17 22 AM" src="https://github.com/ranjitaelizabeth/test/assets/33226052/123cd19c-46ec-4c38-91b1-c69148062c1e">


