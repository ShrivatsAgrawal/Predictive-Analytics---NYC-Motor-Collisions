# Predictive Analytics on NYC Motor Collisions

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
[![LinkedIn][linkedin-shield]][linkedin-url2]
[![LinkedIn][linkedin-shield]][linkedin-url3]

<!--[![MIT License][license-shield]][license-url]-->

<p align="center">
  <img src="https://media.giphy.com/media/8uiZLn37DZIXu/giphy.gif" alt="animated" />
</p>

<!-- MOTIVATION -->
## Motivation



Is NYC a secure walking city? Are people frightened of getting hit by cars? Which borough has deadly collisions? Are motorists injured more than cyclists? How many of injuries result in deadly deaths?

Considering many situations above, will the collisions result in injuries and deaths of people? We believe we can reduce injuries and deaths by utilizing the open data available and help users with effective insights beforehand and factors resulting in collisions.


<!-- ABOUT THE PROJECT -->
## Introduction

[![Product Name Screen Shot][product-screenshot]](https://anushkasandesara.medium.com/predictive-analytics-on-nyc-collision-data-9f06c94140f2)

A New York Times [article](https://www.nytimes.com/2021/09/30/nyregion/traffic-deaths-nyc.html) reported that streets in New York have grown more precarious because deaths and fatalities due to traffic collisions have risen 10.5 percent to 8,730 in the first 3 months of 2021 from 7,900 deaths in the same period in 2020. As New York city is home to more than 8 million people and approximately 45 million people visit every year the traffic will surge which can cause more collisions. The objective of this project is to <b>gather insights, perform comprehensive exploratory data analysis to understand the relationship between various features of the dataset and use them to make better machine learning predictive models.</b>


<p align="right">(<a href="#top">back to top</a>)</p>

## Built With

Here are the awesome tools we used:

* [Python3](https://www.python.org/download/releases/3.0/)
* [Matplotlib](https://matplotlib.org/)
* [Seaborn](https://seaborn.pydata.org/)
* [Folium](https://python-visualization.github.io/folium/)
* [Scikit-learn](https://scikit-learn.org/stable/)
* [Plotly](https://plotly.com/)
* [Geopandas](https://geopandas.org/en/stable/)
* [Wordcloud](https://pypi.org/project/wordcloud/)

<p align="right">(<a href="#top">back to top</a>)</p>


## Datasets

The [dataset](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95) contains information about collisions reported in NYC by the police department. The dataset contains 1.84M rows and 29 columns latest updated as of 7th November. Based on our analysis from the website the dataset contains columns like <b>crash date, time, location, borough, collision id, number of persons injured, number of pedestrians injured, number of pedestrians killed, number of cyclists killed, number of cyclists injured, contributing factors behind the collision, vehicle types and many other relevant features.</b> <br><br>
Furthermore, we scraped weather data from this [website](https://www.wunderground.com) which contains information on <b>temperature, wind, humidity, windspeed, wind gust, pressure, precipitation and condition.</b>

<b> Google Drive <a href = 'https://drive.google.com/drive/folders/1WNSEIY1K3WzlmpFx6l89S3em4XkTiKId?usp=sharing'>Link</a> to Access our Collision Data and Scraped Weather Data </b>


<!-- ROADMAP -->
## Roadmap

[![Roadmap][roadmap]](https://anushkasandesara.medium.com/predictive-analytics-on-nyc-collision-data-9f06c94140f2)

See the [open issues](https://github.com/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONCLUSION -->
## Conclusion

New York is sometimes called the biggest collection of villages in the world. This is the reason why this project and the datasets caught our attention. 
A city that is known for its hustle and bustle also inevitably leads to collisions. 
With this project we embarked on a journey to uncover the patterns behind these collisions and the factors that might contribute to them. Ultimately we wanted to propose a solution which could help in reducing the number of accidents by suggesting preventive measures.

We started off with the project by collecting the collision data from [Motor Vehicle Collisions - Crashes | NYC Open Data](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95) and scraping weather information from [Weather Underground](https://www.wunderground.com/). This enabled us to get an overview of the weather conditions at the time of the collision and whether they had an effect in any way.

Next up, the data was wrangled and pre-processed to deal with null values, duplicates and remove columns not offering much information.
After getting the data into a clean, easy to use format various informative visualizations were made using the data. Some of the examples include Bar Charts for showing the number of collisions with respect to the contributing factors and the different weather conditions, borough wise spread of the collisions, interactive line charts for visualizing how the time of the day had an effect on the number of collisions, 3D movable geo plots for visualizing the collision density on each street in the city and many more.

We derived several useful insights from these visualizations like:
1. Motorists were most likely to be involved in accidents
2.  Brooklyn leaded the charts in terms of number of collisions
3. Driver distractions was the leading cause of collisions
4.  More than 60% of the accidents occurred when the weather was cloudy
5. Across all the boroughs more collisions occurred on the weekdays than the weekend and that too  between 8AM and 5PM


We believe that we were able to uncover many important facts and patterns about the collisions in NYC which will assist in putting preventive measures in place and lead to safer roads.

After visualizations and EDA we proceeded on to modeling the dataset with Unsupervised and Supervised learning techniques to be able to draw predictions on whether given the weather conditions and time of the day, are the accidents likely to be severe or not. In other words, whether the accident will result in injuries. 

We trained the Supervised learning models on the training data. Models used were Logistic Regression model, Random Forest model and Stacking with K-Nearest Neighbor, Decision Tree and Logistic Regression model. Later these trained models were used to make predictions on the test data with an accuracy of around 80%. The dataset had imbalanced labels so we also downsampled our data inorder to attain equal number of 0’s and 1’s in the target variable. On training and predicting the models on this downsampled data, we got an accuracy of around 54%.

With the conclusion of modeling, we were able to build a classifier which can help the authorities put precautionary measures in place to prevent collisions from happening by putting speed, vehicle size restrictions etc. when the likelihood of severe collisions is more.


<!-- FUTURE SCOPE -->
## Future Scope

In this project, we did not have time series geospatial information regarding normal traffic activity. This data can prove to be very useful for charting out routes to avoid collision prone areas. Our future efforts can be directed to obtaining this information and using it to build a guidance system for the average New Yorker for safer road journeys. 

In addition, more information about the people involved in the collision can be used by the authorities to improve their process of issuing driver licenses and changing driver tests.


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

Shrivats Agrawal - <a href='https://www.linkedin.com/in/shrivats-agrawal/'> LinkedIn </a> - shriv9@seas.upenn.edu <br>
Anushka Sandesara - <a href='https://www.linkedin.com/in/anushka-sandesara/'>LinkedIn</a> - anu12@seas.upenn.edu <br>
Dhruvi Modi - <a href='https://www.linkedin.com/in/dhruvi-modi-093a93155/'>LinkedIn</a> - dhruvim@seas.upenn.edu <br><br>
Project Link: [https://github.com/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions/](https://github.com/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions/)<br>
Medium : [Link](https://anushkasandesara.medium.com/predictive-analytics-on-nyc-collision-data-9f06c94140f2)
<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments


<b>Our TA and mentor, [Tashweena Heeramun](https://www.linkedin.com/in/tashweena-heeramun-6a4237189/) who constantly provided us with support and guidance.
 [Prof. Zachary Ives](https://www.cis.upenn.edu/~zives/) for providing us with the concepts we needed to be confident enough to explore different areas in Big Data Analytics to get the best out of this course and project.</b>
<p align="right">(<a href="#top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions.svg?style=for-the-badge
[contributors-url]: https://github.com/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions.svg?style=for-the-badge
[forks-url]: https://github.com/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions/network/members
[stars-shield]: https://img.shields.io/github/stars/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions.svg?style=for-the-badge
[stars-url]: https://github.com/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions/stargazers
[issues-shield]: https://img.shields.io/github/issues/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions.svg?style=for-the-badge
[issues-url]: https://github.com/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions/issues
[license-shield]: https://img.shields.io/github/license/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions.svg?style=for-the-badge
[license-url]: https://github.com/ShrivatsAgrawal/Predictive-Analytics---NYC-Motor-Collisions/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/shrivats-agrawal/
[linkedin-url2]: https://www.linkedin.com/in/anushka-sandesara/
[linkedin-url3]: https://www.linkedin.com/in/dhruvi-modi-093a93155/
[product-screenshot]: images/nyc.png
[roadmap]: images/roadmap.png
