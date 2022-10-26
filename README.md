# The repository being analyzed is [311 Service Requests](https://data.cityofchicago.org/Service-Requests/311-Service-Requests/v6vf-nfxy/data)  

The dataset has 7,017,021 rows and 2.28GB. We selected a subset of rows of request type: "Water On Street Complaint", reducing the dataset to 31,963 rows.
 
311 is a service for non-emergency issues and requests. This quote from the website examplifies it: "You can call 311 to find out what Police District and beat you live in, as well as the date, time and location of your next beat meeting. Contacting 311 gives you easy access to non-emergency police services, from filing police reports to talking to police personnel in your district."

## Problem

Urban flooding is a serious phenomena that can affect the well being of the city's citizens. It can damage public structures, natural structures like trees, private belongings (such as houses and cars), it can hinder city navigation, cause a traffic jam, help spread deseases like leptospirosis and increase the chances of all sorts of accidents. In order to solve this problem it is necessary to investigate the patterns of urban flood, since this problem is heavly associated with how the city is structured, mainly the streets. That being said, in order to investigate the problem we filtered the dataset by requests of type: "Water On Street Complaint".  

### Question 1

**Domain question:** How does the position of the street influences flooding?

**Data question:** How is the distribution of "Water On Street Complaint" grouped by street and street direction comparing the last three years (using unified color scale)?

**Atributes:** street number, street direction, request type, created date

This question can help us understand if the urban floods are related to the water flow in the city. Besides that, situations like climate change can make this water flow change and places that were less affected by the rains become more affected and vice versa. Being able to compare the absolute number of requests over time is also important, because it allows the prediction of a more accurate future cenario that can guide the decisions to tackle the problem.

The attributes selected are the ones necessary to answer the data question. The "request type" because we want to filter only the requests associated with our problem. The street direction because we want to understand how floods are affected by the positions of the street. Created date because we want to do the comparison over time. The street number because we want to group the data geographically by street.

### Question 2

**Domain question:** How much rain is considered a problem by the citizens?

**Data question:** How is the rain precipitation related to the number of "Water On Street Complaint" throughout the last three years?

**Atributes:** created date, rain precipitation, request type (number of requests) 

Flooding is obiviously correlated to the rain precipitation. However, it is important to have an overview of how susceptible is the city to rain. It is also important to do this analysis over time to notice how the city has developed over the years. Becoming less susceptible, more susceptible or not changing.

The created date attribute was selected because we want to do a comparison over time. The rain precipitation by day is an attribute that comes from another dataset and indicates the volume of rain in one day. The request type because we want to filter the data by "Water On Street Complaint".

### Question 3

**Domain question:** How does the structure of the street influences flooding?

**Data question:** How does street direction and street type influences the amonut of "Water On Street Complaint" considering all data from the last three years?

**Atributes:** street direction, request type (number of requests), street type

This is an extention of question 1. It is important to investigate how the structure of the street influences ocurrency of flooding. Since it is possible to drive more useful conclusions about what types of interventions are most likely to succeed.

Street direction indicates an important aspect of the structure of the street as well as street type, since width, material and purpose can all be deducted from this attribute. Finally, the request type is necessary to filter the data to only consider "Water On Street Complaint".

## Some other possible domain questions

Are water on street complaints associated with socio-demographic aspects?
Does the pattern of floods change throughout the years?
How much rain is considered a flood by citizens throughout the city?
What are the most fragile regions susceptible for floods?
Is the electrical district susciptible to flooding?
What are the most possibly affected electricity grids?
What are the regions susceptible to electricity problems?
What types of areas are more susceptible to flooding (residential, commercial, ...)?
How is the flooding distributed between streets? 
How does street type affect flooding?
What are the regions susceptible to electricity problems?