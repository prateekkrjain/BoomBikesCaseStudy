# BoomBikes Case Study
> To build a Linear Regression model to understand the factors which influence the demand.

## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Contact](#contact)

## General Information
> A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

> In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

> The purpose of this case study is to model the demand for shared bikes with the available independent variables. It will help the management to understand how exactly the demands vary with different features. They can then accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. 

> Further, the model will be a good way for management to understand the demand dynamics of a new market. 

## Conclusions
+ R_squared & Adjusted R_squared both are close to 82%, hence the model contains right amount of variables
+ Constant: that is base demand is 4,685.34
+ Light rain and snow that is when there is any rain or snow, it has negative impact on negative impact on the demand, that is, it reduces demand by 2,093.85. Also, this has the highest impact on the demand.
+ Year also have significant coefficient of 992, indicating that in 2019 demand is higher by 992 as compared to 2018.
+ Temperature have a positive coefficient value indicating that as the temperature rised more people demand for the ride. It could be due to the fact that people may not prefer to walk or take public transport during high temperatures. Its coefficient is 935 i.e. unit change in temperature will lead to rise in demand by 935.
+ Winters also lead to higher demand as people might not prefer to walk in cold. It has coeffient value of 732, that is in winters demand rised by 732.
+ Spring season and Mist or Cloudy weather have negative impact on the demand. In spring demand reduced by ~800, while in Cloudy weather it reduces by ~400 bookings
+ All the other coefficients are also statistically significant

## Technologies Used
- Python - version 3.8.3
- Numpy - version 1.18.5
- Pandas - version 1.0.5
- Seaborn - version 0.11.0
- Wordcloud - version 1.8.1
- Matplotlib - version 3.2.2
- Statsmodel - version 0.11.1

## Contact
Created by [@prateekkrjain](http://prateekkrjain.com) - feel free to contact me!)





=========================================
Dataset characteristics
=========================================	
day.csv have the following fields:
	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered
	
=========================================
License
=========================================
Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}

=========================================
Contact
=========================================
	
For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt)
