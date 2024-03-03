## Python_API_Challenge
-------------------------------------------------------------------------------------------
Background
-------------------------------------------------------------------------------------------
Data's true power is its ability to definitively answer questions. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"

Now, we know what you may be thinking: “That’s obvious. It gets hotter.” But, if pressed for more information, how would you prove that?

-------------------------------------------------------------------------------------------
Technologies Used
-------------------------------------------------------------------------------------------
- Python
- Pandas libraqry
- Jupyter Notebook
- Matplotlib library
- Citipy

-------------------------------------------------------------------------------------------
API's Utilized
-------------------------------------------------------------------------------------------  
- OpenWeatherMap API
- Google Places API
  
-------------------------------------------------------------------------------------------
Instructions
-------------------------------------------------------------------------------------------
Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and your problem-solving skills to create a representative model of weather across cities.

For this part, you'll use the WeatherPy.ipynb Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:
  - Latitude vs. Temperature
  - Latitude vs. Humidity
  - Latitude vs. Cloudiness
  - Latitude vs. Wind Speed

Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.

Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values as you can see in the following image

![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/efe24683-126a-496f-b399-8246b899ad9f)
![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/4f76d175-e168-4dec-8175-86fd931c3b5b)
![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/972261c4-7b95-49a3-9ec8-ad3eecdd3d2c)
![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/a889ce86-b91d-45a1-9772-7180bfa1df23)
![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/cb00bd1c-6e64-4cfd-9c6b-413036e2f221)
![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/6396cfea-629b-4e1c-8017-8d3d837dae01)
![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/a8504984-ce9c-49a5-804c-7f6159488389)
![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/f939ebbf-13dc-4382-90f9-a19a04fbc2e2)

Part 2: VacationPy
In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/c98b7f8d-cb3c-4979-be7d-6dc22825a70d)
Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
- A max temperature lower than 27 degrees but higher than 21
- Wind speed less than 4.5 m/s
- Zero cloudiness

NOTE
Feel free to adjust your specifications but make sure to set a reasonable limit to the number of rows returned by your API requests.

Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

![image](https://github.com/lleiva25/Python_API_Challenge/assets/140974405/2b4d6929-a94d-47a7-b2e6-a7393c3ec4b6)

-------------------------------------------------------------------------------------------

