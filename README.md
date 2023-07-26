# python-api-challenge

## Starter Code
For this assignment, I chose to work with the starter code provided so that I had a solid foundation for building the key components of this homework. I did not put the WeatherPy.ipynb and the VacationPy.ipynb files in their own individual folders as this would cause the code I have written for saving PNG's and accessing the created csv to error. By placing all files in the same directory as the .gitignore, I also resolved the error created when importing the api keys, as trying to import them from within a separate folder was not working.

## Import os to make new folder
I was unsure how the code would be run in order to grade this assignment, as there was not already an output_data folder created in my repository to save the PNG's to. I solved this by importing os and added a line of code to check for the presence of the output_data folder. If the folder exists, then the PNG's will save to it. If the folder does not exist, the folder will be created and then the PNG's can be saved to it. I referenced the link below for help with this.

Link: https://stackoverflow.com/questions/59487696/check-if-a-folder-exists-in-a-given-path-and-if-not-then-create-a-folder-there
