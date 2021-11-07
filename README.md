1 R Project: Analysis of Olympic Games data
Oxana Kolpakova

Data description: This is a historical on the modern Olympic Games, including all the Games from Athens 1896 to Rio 2016. The athlete events dataset contains information about Olympic Athletes and events that they have competed in, including biological data (Age, Sex, Height, Weight etc.) and event data (Year, Season, City, Sport etc.). The NOC (National Organizing Committee) regions dataset possesses information about the countries that compete in the Olympics, including the country name and any notes about said country.

The file processed_data.csv contains 271115 rows and 15 columns. Each row corresponds to an individual athlete competing in an individual Olympic event. 
The Athletes dataset contains 15 variables:
1.	ID: A number used as a unique identifier for each athlete 
2.	Name: The athlete’s name(s) in the form of First Middle Last where available 
3.	Sex: The athlete’s gender; one of M or F Age: The athlete’s age in years 
4.	Height: The athlete’s height in centimeters (cm) 
5.	Weight: The athlete’s weight in kilograms (kg) 
6.	Team: The name of the team that the athlete competed for 
7.	NOC: The National Organizing Committee’s 3-letter code 
8.	Games: The year and season of the Olympics the athlete competed in in the format YYYY 
9.	Year: The year of the Olympics that the athlete competed in 
10.	Season: The season of the Olympics that the athlete competed in 
11.	City: The city that hosted the Olympics that the athlete competed in 
12.	Sport: The sport that the athlete competed in 
13.	Event: The event that the athlete competed in 
14.	Medal: The medal won by the athlete; one of Gold, Silver, or Bronze. NA if no medal was won. 

Task: In this project we had corrected the incoming data, analyzed it according to several required parameters and made EDA

Steps of analyses:
1.	Load the necessary libraries. 
2.	Import data sets. 
3.	 Check whether there are missed or non-valid values, fixed them. 
4.	We answered the questions asked by the project №№ 3-16:
  •	Age of youngest athletes of both genders at the 1992 Olympics. 
  •	Mean and standard deviation of type Height for
  •	Mean and standard deviation of female tennis players' height at the 2000 Olympics. 
  •	What sport did the heaviest athlete participate in at the 2006 Olympics?
  •	How many gold medals were won by women from 1980 to 2010? 
  •	How many times has athlete John Aalberg competed in the Olympics over the years?
  •	The least and most represented by the number of participants age groups of athletes at the 2008 Olympics. 
  •	How has the number of sports in the 2002 Olympics changed from the 1994 Olympics?
  •	3 Top of countries for each type of medal for the Winter and Summer Olympic Games 
  •	Create a new variable Height_z_scores and store the values of the Height variable in it after it's 
  •	Create a new variable Height_min_max_scaled and
  •	store the values of the Height variable into it after applying min-max normalization to it.
  •	Compare the height, weight and ages of men and women who competed in the Winter Olympics.
  •	Whether there is a correlation between the variables Team and Medal?
  •	EDA. We build a linear regression model of the relationship between the number of medals, gender and age.



