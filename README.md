Rescue to Rescuer
# Overview

This project is a web-based dashboard built using Plotly Dash and Dash Leaflet for visualizing animal data from a MongoDB database. It includes interactive features such as data tables, maps, and pie charts for filtering and viewing data related to different rescue types (Water Rescue, Mountain or Wilderness Rescue, Disaster, or Individual Tracking).

## Why MongoDB?

MongoDB was chosen for its document-oriented storage model that aligns seamlessly with Python’s data structures, allowing flexible and dynamic schema management. Its high performance and scalability are crucial for handling large datasets and high-throughput operations. MongoDB’s robust querying capabilities, including geospatial queries and aggregation, enable efficient data retrieval and manipulation, making it ideal for interactive and responsive dashboards like this one. The integration with Python through the PyMongo library provides a powerful and intuitive way to interface with the database, facilitating rapid development and efficient data management. [MongoDB installation guide]( https://www.mongodb.com/docs/manual/installation/).

## Dash Framework

The Dash framework, developed by Plotly, is a powerful tool for building interactive, web-based data visualization applications. It combines the capabilities of Flask for the web server, Plotly for interactive graphs, and React.js for responsive user interfaces. Dash abstracts much of the complexity involved in web development, allowing Python developers to create sophisticated dashboards with minimal effort. [Dash Python User Guide](https://dash.plotly.com).

## Features

Dynamic Data Table: Displays animal data with the ability to sort and filter.
Interactive Map: Shows animal locations based on selection or filter criteria.
Pie Chart: Visualizes breed distribution, updating according to filter selections.
Responsive Layout: Works on various screen sizes.

## Getting Started
Before beginning, ensure you have the following installed on your local machine.
1.	Python 3.x: The main programming language used in this project. Download from [Python.org](https://www.python.org/downloads/). 
2.	Installing pip: ‘pip’ is the package installer for Python, used to install and manage software packages written in Python. If ‘pip’ is not already installed with your Python distribution, follow these steps:
a.	Check if pip is installed: Open your terminal or command prompt and type:
```bash
pip –version
```
![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/f9cfae15-5193-421a-a5f4-bdd74370d39e)

b.	Install pip: If pip is not installed, run the following commands in the terminal (then repeat step 2.a):
```bash
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python3 get-pip.py
‘’’
3.	MongoDB Server: The database used to store and manage the data. Follow the installation instructions on [MongoDB installation guide]( https://www.mongodb.com/docs/manual/installation/).
4.	Install all required Python packages:

```bash
pip install pandas numpy matplotlib plotly dash dash-leaflet jupyter-dash notebook
```
## Setup

1.	Clone the repository:
```bash
git clone https://github.com/YourUsername/SNHU-CS-340-Dashboard.git
cd SNHU-CS-340-Dashboard
```

2.	Database Configuration:
a.	Ensure your MongoDB instance is running and accessible. Update the connection details in `animal_shelter.py` and the dashboard script.

## Usage

# Starting the Dashboard

1.	Ensure MongoDB Server is Running:
a.	Before Starting the dashboard, make sure your MongoDB server is up and running. You can start it using the following command in your terminal. 
```bash
mongo sh
use aac
```
 

b.	If you need guidance on setting up MongoDB, refer to the [MongoDB installation guide]( https://www.mongodb.com/docs/manual/installation/).

2.	Launch the Dashboard:

a.	Navigate to the directory containing your project:
```bash
cd path/to/SNHU-CS-340-Dashboard
```
b.	Open the Jupyter Notebook:
```bash
Jupyter notebook
```
c.	Open the `ProjectTwo.ipynb` file in Jupyter Notebook and run all cells. This will start the dash server. 
 
Cell 1

 ![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/b4594f06-18ac-4097-ae04-8b9625a3d94f)

Cell 2

 ![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/01225162-673b-4095-a1a2-386f47457e30)

Cell 3

![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/ae285ee9-a0f0-4536-b0d1-41b5623d765e)
 
Cell 4

 ![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/b9a29990-aaec-4558-9f22-b038c76ed762)

Cell 5

![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/60f3d8df-3f84-40c2-bef4-2391487ab6b7)
 
Cell 6

 ![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/184aa8f0-4c30-4685-88cd-f364a15fba34)

Cell 7

![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/f5e3fd83-34e6-477e-a152-1e17d402fc3b)
 
## Using the Dashboard

The dashboard will load in the default settings, with no filters applied.

![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/6463de6b-bf84-4633-9317-51d10e3615b8)
  
![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/6fefe32c-367f-4238-a0f7-14d2c2ca8064)
 
You can filter the results through four different options.
1.	Water Rescue

 ![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/3db0ba14-ea12-4e46-aba0-d84872d6f2d3)

![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/90db7de0-246a-4fc5-8ca8-ae9ba9bbcee9)
 
2.	Mountain or Wilderness Rescue.

 ![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/1be9f1bc-bffb-49a9-89bc-be225a2e84ff)

![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/1fd6b220-d083-48ae-827b-6c9cc11b0d8b)

3.	Disaster or Individual Tracking.

 ![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/e763b94c-6ce6-4ccf-a8e5-eb94242d35c7)

 ![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/b4cc6a18-6dbc-4bd1-b576-c4eae59bba88)

4.	Lastly, you can filter using the table in any column.

 ![image](https://github.com/Joseph-Les/AnimalRescueDashboard/assets/84045743/5a6a3238-8fbf-464d-8022-72d91031c934)

## Troubleshooting:

1.	Common Issues: If you encounter issues connecting to MongoDB or performing operations, check the following:
a.	Ensure MongoDB server is running and accessible.
b.	Verify that the connection details (username, password, host, port, database, and collection) are correct.
2.	Debugging Tips:
a.	Use print() statements to debug issues by displaying variable values and results at various stages.

How do you write programs that are maintainable, readable, and adaptable? What were the advantages of working in this way? How else could you use this CRUD Python module in the future?

1.      To write programs that are maintainable, readable, and adaptable, it’s essential to follow best practices such as modular design, clear and consistent naming conventions, thorough documentation, and comprehensive testing. In Project One, the CRUD Python module was designed to interact with the MongoDB database efficiently. This module was reusable and provided a clean interface for database operations, which made connecting the dashboard widgets in Project Two straightforward and seamless. The module can be extended to support additional database operations or new types of queries. It can be integrated into other applications that require database connectivity, such as web services or data analysis tools. Lastly, serves as a teaching tool for illustrating how to implement and use CRUD operations with MongoDB in Python.

How do you approach a problem as a computer scientist? Consider how you approached the database or dashboard requirements that Grazioso Salvare requested. How did your approach to this project differ from previous assignments in other courses? What techniques or strategies would you use in the future to create databases to meet other client requests?

1.       As a computer scientist, I approach problems by systematically breaking them down into manageable components, conducting thorough analysis, and applying best practices in design and development. For Grazioso Salvare's database and dashboard requirements, I began by understanding their needs, designing a MongoDB schema, and creating a reusable CRUD Python module for database interactions. This modular approach ensured that the database operations were efficient and easily integrated into the interactive dashboard built using Dash. Compared to previous assignments, this project emphasized real-world application, requiring a comprehensive understanding of both backend and frontend development. In future projects, I will employ techniques such as requirement workshops, prototyping, agile development, scalability considerations, and robust security practices. This ensures that databases and applications are not only effective and efficient but also scalable, secure, and tailored to meet specific client needs.

What do computer scientists do, and why does it matter? How would your work on this type of project help a company, like Grazioso Salvare, to do their work better?

1.       Computer scientists design and develop software systems to solve problems and improve technology and business operations. This work matters because it drives innovation, enhances productivity, and supports data-driven decision-making.

2.       For a company like Grazioso Salvare, my project helps streamline data management and improve operational efficiency. By creating an interactive dashboard integrated with a robust database, staff can efficiently track and analyze animal data, monitor rescue operations, and make informed decisions. This leads to better resource allocation and supports their mission of rescuing and caring for animals.

## License

[MIT](https://choosealicense.com/licenses/mit/)

Contact:
Joseph Les
