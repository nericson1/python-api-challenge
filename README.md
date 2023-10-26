# python-api-challenge

## Description
The OpenWeatherMap API was called to gather weather information such as temperature, humidity, cloudiness, and wind speed across varying cities. Linear regression models were created for each of these factors. This information was then used to create a series of maps displaying cities gathered from the API, as well as hotels within cities meeting a certain weather criteria.

I did not put the WeatherPy.ipynb and the VacationPy.ipynb files in their own individual folders (per instrunctions) as this would cause the code I have written for saving PNG's and accessing the created csv to error. By placing all files in the same directory as the .gitignore, I also resolved the error created when importing the api keys, as trying to import them from within a separate folder was not working.

## References
### Prior class activities and challenges
For this assignment, I primarily relied on previous challenge assignments and activities I have completed for code reference. I use the code I wrote for linear regression modeling in the module 5 challenge as a base for writing my linear regression model function in this assignment. I also used many of my notes from module 6 to compile the code I wrote on this assignment for creating my scatterplots and maps.

### Import os to make new folder
I was unsure how the code would be run in order to grade this assignment, as there was not already an output_data folder created in my repository to save the PNG's to. I solved this by importing os and added a line of code to check for the presence of the output_data folder. If the folder exists, then the PNG's will save to it. If the folder does not exist, the folder will be created and then the PNG's can be saved to it. I referenced the link below for help with this.

Link: https://stackoverflow.com/questions/59487696/check-if-a-folder-exists-in-a-given-path-and-if-not-then-create-a-folder-there

### df.iterrows and df.at
After getting our data through the API, the Max Temp is stored in Kelvin, but I need to display the temperature data as Celsius. I needed to iterate through the dataframe and take the Max Temp value, and I used the df.iterrows() fuction to do this, as I have before. However I needed to also include df.at[index, 'Max Temp'] in order to run a calcuation on the value in my dataframe to change it to Celsius. I referenced the link below for help with this.

Link: https://stackoverflow.com/questions/23330654/update-a-dataframe-in-pandas-while-iterating-row-by-row
