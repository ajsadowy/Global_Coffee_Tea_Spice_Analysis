# Global Coffee, Tea, and other Spices Analysis   
"He who controls the spice controls the universe."
A great line from a great Sci-Fi classic Dune, our world is run on spice. Not necessarily the galatic fuel for space travel, but the type that gives us additional flavors to our culinary tastes as wells as providers of unique organic molecules used for health and personal energy benefits. The goods are consistantly traded around the world and with consistant demand it seems like an interesting topic for further statistical analysis.   

## Project Overview   
The purpose of this project is to explore global import and export data of common coffee, tea, and other spices/herbs. We choose this topic because these trade goods are a staple to our modern world.    

### Process   

#### Data Collection   
We gather data from [UN Data website](http://data.un.org/Default.aspx), a great repository for data files on global topics. Specifically [here]( http://data.un.org/Data.aspx?d=ComTrade&f=_l1Code%3a10), we were able to download the csv files on the topic of global trade on coffee, tea, mate, and spices.   

On this site we came across our first obstacle, the site had a limitation of how large the csv file can be downloaded. Luckily the site allows for filtering the data based on topics like trade goods, country of origins, and year. We were able to get the complete data by downloading seperate csv files based on trade goods. With this we had workable csv files.   
From these three files were were able to join them into one easy to load csv file.   

#### Exploratory Analysis
With the csv files we began exploring the data with utilizing Tablaeu to get some interpretable visualizations of the data.   
#### Preperation of the Data and Database Storage   
One issue with setting up the postgres SQL database is transforming the data types of the csv file to a usable format to upload to the database. Our attempt was to follow a python script created by [Nate from StrataScratch](https://github.com/Strata-Scratch/csv_to_db_automation). With this script we could update the datatypes on our csv files to a usable datatype encoding to upload a df to our database.

To host the database we attempted to use Amazon Web Services (AWS).   

Unfortunately, when attempting to run our script we recieved an error message with being timed out from connecting AWS. Troubleshooting is necessary for the future by contacting AWS customer support.   
#### Machine Learning Models   
* Unsupervised Machine Learning   
* Neural Network Model

#### Conclusions

### Resources   
* [UN Data for Trade Goods](http://data.un.org/Default.aspx)   
* [Nate from StrataScratch Python Script](https://github.com/Strata-Scratch/csv_to_db_automation)
* 
### Project Team Members   
* [Adam Sadowy](https://github.com/ajsadowy)   
* [Thi Ngo](https://github.com/Thingo2906)   
* [Olena Rabani](https://github.com/olenarabani)   
* [Josie Boyer]()   
* [Shawn Toosi]()
### Team Communication
* Slack - Most direct form of communication when working.   
* Zoom  - Biweekly meetings to see where everyone is with the project.   
* Group Text Group - Direct communication when away from project.   
* Discord - Back up communication if Zoom were to fail.   
