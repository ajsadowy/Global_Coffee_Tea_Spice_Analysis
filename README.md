# Global Coffee, Tea, and other Spices Analysis   
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/Images/40941991-2416-4bbc-95bd-40b1d55011b9.jpg)   
"He who controls the spice controls the universe."
A great line from a great Sci-Fi classic Dune, our world is run on spice. Not necessarily the galatic fuel for space travel, but the type that gives us additional flavors to our culinary tastes as wells as providers of unique organic molecules used for health and personal energy benefits. The goods are consistantly traded around the world and with consistant demand it seems like an interesting topic for further statistical analysis.   

## Presentation Slides  
[Google Slides](https://docs.google.com/presentation/d/1ar_TVjZ9b3tX65JqmfR_XULhvNhESwEjbGiwPGQnDaQ/edit?usp=sharing)   

## Project Overview   
The purpose of this project is to explore global import and export data of common coffee, tea, and other spices/herbs. We choose this topic because these trade goods are a staple to our modern world. 
 Coffee and spices are an integral part of our life. Isn't morning coffee and news the beginning of every movie? At home, in the office, when meeting with friends, we enjoy a cup of aromatic coffee. Our dishes are enriched with new flavors thanks to various spices both at home and in restaurants. Special small shops are opened that specialize in different types of coffee, or a variety of spices.
 Accordingly, the export-import analytics of these goods is very interesting.

For analysis, our team used programs such as:

-PostgreSQL

-Tableau

-Jupyter Notebook python

-HTML

-Google Slides

Thanks to this analysis, we wanted to trace how export-import changed with the change of century and the development of delivery routes. How countries appeared and disappeared in the world market. How the volume of export-import changed in different years. Which countries have been and remain dominant in the supply of coffee / tea and spices.


### Process   

#### Data Collection   
We gather data from [UN Data website](http://data.un.org/Default.aspx), a great repository for data files on global topics. Specifically [here]( http://data.un.org/Data.aspx?d=ComTrade&f=_l1Code%3a10), we were able to download the csv files on the topic of global trade on coffee, tea, mate, and spices.   

On this site we came across our first obstacle, the site had a limitation of how large the csv file can be downloaded. Luckily the site allows for filtering the data based on topics like trade goods, country of origins, and year. We were able to get the complete data by downloading seperate csv files based on trade goods. With this we had workable csv files.  
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/Images/QuickDBD-export.png)   

From these three files were were able to join them into one easy to load csv file.   

#### Exploratory Analysis
With the csv files we began exploring the data with utilizing Tablaeu to get some interpretable visualizations of the data.   
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/Tablaeu_Images/THE%20TOP%2010%20TRADING%20(BY%20WEIGHT-KG)%20COUNTRIES.png)   
#### Preparation of the Data and Database Storage   
One issue with setting up the postgres SQL database is transforming the data types of the csv file to a usable format to upload to the database. Our attempt was to follow a python script created by [Nate from StrataScratch](https://github.com/Strata-Scratch/csv_to_db_automation). With this script we could update the datatypes on our csv files to a usable datatype encoding to upload a df to our database.
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/Images/clean.png)   
To host the database we attempted to use Amazon Web Services (AWS).   

Unfortunately, when attempting to run our script we recieved an error message with being timed out from connecting AWS. Troubleshooting is necessary for the future by contacting AWS customer support.   
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/Images/Untitled.png)   
#### Machine Learning Models   
* Unsupervised Machine Learning   -
Our goal for this model was to discover possible trends in the world of the spice trade. Using an unsupervised machine learning and clustering algorithms to find patterns whether a good is imported, exported, re-imported, or re-exported.   

![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/MachineLearning/Unsupervised/ML_IMAGES/BlackTeaElbow.png)   
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/MachineLearning/Unsupervised/ML_IMAGES/TeaBlack3D.png)   
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/MachineLearning/Unsupervised/ML_IMAGES/TeaGreen2D.png)   
* Neural Network Model   
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/Images/NN.png)

#### Conclusions   
Seeing similar trends of clustering for most spice trade goods with this data we may be able to set up a minimum cost and maximum profit models with just the additional information for shipping costs.   
Coffee (Roasted) Cluster Model:   
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/MachineLearning/Unsupervised/ML_IMAGES/coffee%203d%20plot.png)

Mate Cluster Model:   
![pic](https://github.com/ajsadowy/Global_Coffee_Tea_Spice_Analysis/blob/PossibleFinal/MachineLearning/Unsupervised/ML_IMAGES/Mate3D.png)   

### Resources   
* [UN Data for Trade Goods](http://data.un.org/Default.aspx)   
* [Nate from StrataScratch Python Script](https://github.com/Strata-Scratch/csv_to_db_automation)
* [Using Unsupervised Machine Learning from Our Cryptocurrency Analysis](https://github.com/ajsadowy/Cryptocurrency_Analysis)   
### Project Team Members   
* [Adam Sadowy](https://github.com/ajsadowy)   
* [Thi Ngo](https://github.com/Thingo2906)   
* [Olena Rabani](https://github.com/olenarabani)   
* [Josie Boyer](https://github.com/JosieBoyer)   
* [Shawn Toosi](https://github.com/Shawn2C)
### Team Communication
* Slack - Most direct form of communication when working.   
* Zoom  - Biweekly meetings to see where everyone is with the project.   
* Group Text Group - Direct communication when away from project.   
* Discord - Back up communication if Zoom were to fail.   
