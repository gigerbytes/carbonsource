
#Politician, Company, and Researcher Impact Score Database
Collect data on politicians, companies, and researchers. Identify their impact on climate change. Use that data to direct consumers away from parties that have a high negative impact and toward parties that have a high positive impact.


##Important Links  
1. Trello Board: https://trello.com/b/iV377Jzq/carbon-source 
2. Spec Sheet (RFC): https://docs.google.com/document/d/18kNvxdlU6cM6G76LYWRXyilrtB2Zra2A3IAHJPfpi-c/edit  


#Company App/Website
* We have in our database information on three grocery store companies:
  * Company A has a high negative impact score because they freight in all of their produce from the other side of the world instead of sourcing local produce.
  * Company B has a neutral impact rating because they balance their carbon production by powering all of their stored by solar power.
  * Company C has a positive impact rating because they use solar power, only sell local, and do not sell plastic water bottles.
* With this information we allow the community to search for the closest grocery stores that has a positive impact rating.
* If none are found in the area, the user is provided a way to request or show interest in shopping at a grocery store like this. Data is collected and can be used to attract positive impact grocery stores in the users community.


#The Politican Scorecard

Initial Requirements for Minimum Viable Product:

Objectives:

We can create a grading profile for each politician similar to the NRA's gun friendly grading site: https://www.nrapvf.org/grades/. We should probably then display the grade with what factors determined that grade, similar to a skillset(Example: Renewable Energy[50], Recycling[20]). Politicians can also be certified through sponsors such as the Rainforest Alliance. Relationships should be displayed such as Company A donated 50,000 to Senator Doe. 

##Present Climate Change opinion/status of the following:

Big Political figures:

* President/VP
* US Congress
* US Senate
* US House
* State Legislature


## Types of INformation

* Voting Record
* Policies
* Quotes
* Campaign Donations


##Key features:
1.Website:

 	 Robust, relational database for storing numerous entries on various topics.
	 
	 Simple but powerful user search function. 
	 
	 Visual content delivery.
	 
	 Text content delivery.
	 
	Comparing multiple politicians.
	
2. Scraper/ parser + database accessor:

	 Easy functional way to quickly retrieve database items.
	 
	 Scraper that parses articles and documents, and outputs the format nicely to
	 
	 Manual input initially- develop automatic crawler
	 
	 Database accessor that stores sets of entries into the production database

 
## General user stories:
* As a user, so that I can quickly input my search request, I should be able to easily submit my search request to a visible field.


* As a user, so that I can easily interpret the resulting data, I should be clearly presented with both visual and textual information relating to my query.


* As an advanced user, so that I can find what I am looking for more easily, advanced search options should be available. 
(Should we allow db queries?)


* As a visually impaired user, so that I can also use the site, the site should be optimised for readers and colour blindness.


* As a user that is searching for data, so that I can easily access large amounts of carbonsource data, there should be an advanced search option to allow for large data amounts.


* As a maintainer, so that I can quickly submit large amounts of data to the scraper, the interface should be easy to use, and allow for quick submission of data.


* As a maintainer, so that I do not have to format resulting data, the parser should output data in a suitable format for easy manipulation and storage.



