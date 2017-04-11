  API BaaS

* Duration : 30 mins
* Persona : API Team

# Use case
Edge API Services includes a backend-as-a-service (BaaS) solution that provides you with access to a flexible data store and enables you to quickly integrate valuable features into your app, including social graphs, user management, data storage, push notifications, performance monitoring, and more.​
Using API BaaS, you can set up your own cloud-based data platform in minutes instead of months – no server-side coding or back-end development needed. This allows your team to focus on developing the rich features and user experience that truly differentiate your app, rather than on the time-consuming details of implementing core back-end services and infrastructure.

# How can Apigee Edge help?
Using API BaaS, you can set up your own cloud-based data platform in minutes instead of months – no server-side coding or back-end development needed. This allows your team to focus on developing the rich features and user experience that truly differentiate your app, rather than on the time-consuming details of implementing core back-end services and infrastructure


# Pre-requisites
You have an Apigee Edge account 

# Instructions

* Log into to Apigee Edge management UI.
Develop-> API BaaS

This will open up a new window with Apigee BaaS
Click on the develop tab.

* Import the hotels collection: 
Click Collections -> 	Click on the plus collection button 
Copy and Paste the json object in the space below
Give the collection a name of "hotels"

* You can now access the collection at this URL: https://apibaas-trial.apigee.net/{org_name}/sandbox/hotels

Effectively you’ve called the GET API for the ‘hotels’ data collection by calling the above URL. Review the information
presented in JSON format. This is the same information you previously saw on the BaaS portal.

Browse towards the bottom of the response. You’ll notice that by default BaaS provides 10 entities at a time. This can be verified
by looking at the attribute "count" : 10

* Now call the GET API as follows with the limits parameter

http://api.usergrid.com/{your-org}/sandbox/hotels?limit=5

* Lets start exploring the query language built into BaaS. You can call the API like this:

https://apibaas-trial.apigee.net/{your-org}/sandbox/hotels?ql=select%20*%20where%20city=%27Burlingame%27

* Try a few of the following other queries to get a better
understanding of how data querying works in BaaS:

-   select * where hotelRating = 3
-   select * where hotelRating = 3 and city = 'Seattle'
-   select * where hotelRating = 3 or city = 'Seattle'
-   select * where shortDescription contains 'Pike'


# Quiz
* What’s the difference between BaaS and MongoDB?
* Describe a scenario where you would want to leverage BaaS.



# Summary
In this lab you learnt about how to use BaaS to store de normalzed data which can be easily queried over a REST interface


