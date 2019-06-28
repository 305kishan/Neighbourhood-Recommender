# Neighbourhood-Recommender for opening a new business in London, UK

# CONTENTS
-Introduction
-Business Problem
-Data Description 
-Data features
-Methodology
-Results and Discussion
-Conclusion

# Introduction
-London is one among the cities in the world, where a large Indian Population resides.
-It is referred to as  the Arch of the world because of its role as the once world’s most powerful kingdom.
-It has a population of over ten million, making it a megacity and most populous city in United Kingdom.  
-Being a demographically diverse city, the needs of the residents are also increasing rapidly. 
-Hence, any new organization or an existing one should keep up with their pace in supplying the needs of the customers

# Business Problem
-Our customer is ABC Restaurant, which is an International Indian Restaurant Brand and also a market leader. 
-ABC Restaurant has recently planned to expand its business to the United Kingdom, and they want to start this journey from the heart of the UK itself. 
-Given the extremely large size and the population of the city, our customer wants to identify the best neighbourhood area to open its first Indian Restaurant covering the majority of the population and facing least competition from other restaurants. 
-The problem statement will be: Which neighbourhood has most Indian population and has lesser number of INDIAN RESTAUARNT’s?

# Data Description
-The data to be used in this project is not readily available. Hence, the data has been obtained from various sources such as
--Foursquare, which is a local search-and-discovery mobile and web based app which provides search results for its users. 
--Wikipedia, which has the details about the neighborhoods in LONDON. https://en.wikipedia.org/wiki/List_of_areas_of_London
--The geographic coordinates of each location have been obtained through Geopy(https://geopy.readthedocs.io/en/stable/)
--The Indian population in LONDON has been obtained from : https://en.wikipedia.org/wiki/Indian_community_of_London

# Data Features
-As we have to explore and identify the neighbourhoods in the city of London, the London neighbourhood data is the crucial data for this project. 
-The data about each neighbourhood is not readily available, hence we have to scrape the Wikipedia page and obtain the data. 
-In order to obtain the coordinates, we make use of geopy library in Python.
-We also need information about each neighbourhood which is  obtained through FourSquare API.
-The population about each neighbourhood will let us know which neighbourhood is more preferable. 

# Methodology
	--Data Preprocessing
	--Exploratory Data Analysis
 	--Clustering (K-Means Clustering)

    1. Data Preprocessing
    ---Scraping from the Wikipedia page
    ---Obtain coordinates for each location using geopy library
    ---Finding columns with null values and replacing them
    ---Merge the neighbourhood dataset with population dataset
    
    2. Exploratory Data Analysis
    ---Begin by exploring the city and finding the count of neighbourhoods and regions in the city. 
    ---Find the unique venues in each neighbourhood. 
    ---visualize the neighbourhoods using a folium map.
    ---Obtain top 10 venues at each neighbourhood, which will let us know which neighbourhoods lacks in Indian Restaurant.
    ---By opening a new Restaurant in Indian populated regions, more customers will be satisfied and the venture will be successful and         profitable and will lay the foundation for further expansion of company’s chain. Hence, we sort top 10 neighbourhoods based on           maximum Indian Population. 
    
    3. Clustering
    ---Sort the neighbourhoods into five clusters to obtain better insights about each neighbourhood and by that we will know which            cluster of neighbourhoods have more population


