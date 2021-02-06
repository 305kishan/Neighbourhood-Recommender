# Neighbourhood-Recommender for opening a new business in London, UK

# CONTENT
<li>Introduction </li>
<li>Business Problem </li>
<li>Data Description </li>
<li>Data features<br>
<li>Methodology<br>
<li>Results and Discussion<br>
<li>Conclusion<br>

# Introduction
<ol>London is one among the cities in the world, where a large Indian Population resides.<br> </ol>
<ol>It is referred to as  the Arch of the world because of its role as the once world’s most powerful kingdom.<br> </ol>
<ol>It has a population of over ten million, making it a megacity and most populous city in United Kingdom.<br></ol>
<ol>Being a demographically diverse city, the needs of the residents are also increasing rapidly.<br></ol>
<ol>Hence, any new organization or an existing one should keep up with their pace in supplying the needs of the customers.<br></ol>

# Business Problem
<ol>Our customer is ABC Restaurant, which is an International Indian Restaurant Brand and also a market leader. <br></ol>
<ol>ABC Restaurant has recently planned to expand its business to the United Kingdom, and they want to start this journey from the heart of the UK itself. <br></ol>
<ol>Given the extremely large size and the population of the city, our customer wants to identify the best neighbourhood area to open its first Indian Restaurant covering the majority of the population and facing least competition from other restaurants. <br></ol>
<ol>The problem statement will be: Which neighbourhood has most Indian population and has lesser number of INDIAN RESTAUARNT’s?<br></ol>

# Data Description
<ol>The data to be used in this project is not readily available. Hence, the data has been obtained from various sources such as<br></ol>
<ol><b>Foursquare</b>, which is a local search-and-discovery mobile and web based app which provides search results for its users. <br></ol>
<ol><b>Wikipedia</b>, which has the details about the neighborhoods in LONDON. https://en.wikipedia.org/wiki/List_of_areas_of_London <br></ol>
<ol>The geographic coordinates of each location have been obtained through <b>Geopy</b>(https://geopy.readthedocs.io/en/stable/) <br></ol>
<ol>The Indian population in LONDON has been obtained from another <b>Wikipedia Article</b> : https://en.wikipedia.org/wiki/Indian_community_of_London <br></ol>

# Data Features
<ol>As we have to explore and identify the neighbourhoods in the city of London, the London neighbourhood data is the crucial data for this project. <br></ol>
<ol>The data about each neighbourhood is not readily available, hence we have to scrape the Wikipedia page and obtain the data. <br></ol>
<ol>In order to obtain the coordinates, we make use of geopy library in Python.<br></ol>
<ol>We also need information about each neighbourhood which is  obtained through FourSquare API. <br></ol>
<ol>The population about each neighbourhood will let us know which neighbourhood is more preferable. <br></ol>

# Methodology
	<ol>Data Preprocessing</ol>
	<ol>Exploratory Data Analysis</ol>
 	<ol>Clustering (K-Means Clustering)</ol>

    1. Data Preprocessing
    <li>Scraping from the Wikipedia page
    <li>Obtain coordinates for each location using geopy library
    <li>Finding columns with null values and replacing them
    <li>Merge the neighbourhood dataset with population dataset
    
    2. Exploratory Data Analysis
    <li>Begin by exploring the city and finding the count of neighbourhoods and regions in the city. 
    <li>Find the unique venues in each neighbourhood. 
    <li>visualize the neighbourhoods using a folium map.
    <li>Obtain top 10 venues at each neighbourhood, which will let us know which neighbourhoods lacks in Indian Restaurant.
    <li>By opening a new Restaurant in Indian populated regions, more customers will be satisfied and the venture will be successful and         profitable and will lay the foundation for further expansion of company’s chain. Hence, we sort top 10 neighbourhoods based on           maximum Indian Population. 
    
    3. Clustering
    <li>Sort the neighbourhoods into five clusters to obtain better insights about each neighbourhood and by that we will know which            cluster of neighbourhoods have more population


