# Resource Database - Curated Link Collection

In this database, students can search through and sort a list of web links and resources. This application is designed to help students begin research and not be overwhelmed with the amount of things they find on the web when they start investigating a research question. A curriculum designer would input resources into the knack database once and it would automatically be populated on the students' and teachers' websites. Although databases and one-stop editing is not new, it is relatively new in curriculum design to have dynamically changing content without having to edit the HTML of a curriculuar website. Editing a resource from one location and having it push to many locations is a significant innovation in terms of workload and the delivery of relevant content to students.

This app uses Knack (www.knackhq.com) to host the database. The Knack API is used to deliver data from Knack to the GE2 websites. The same database was installed on two separate websites using wordpress (a teacher one and student one), with each having a custom interface. The primary reason I am putting this project on github is the amount of trial and error I had to go through to get PHP to talk to the Knack database API. Knack's documentation for the API on PHP is lacking, especially for a dabbler in programming and web services like me.

I scripted the calls to Knack in PHP. It integrates well with our Wordpress builds and I am more familiar with PHP at this time. The API returns JSON, but can be decrypted into something PHP can use. 

A variety of fields have been included as well for filtering. These were represented as fields in the Knack database. I implemented filters as additions to the GET URL that Knack uses. These are just appended whenever users activate a filter. 

Whenever a filter is applied, an AJAX call is used on the user's page to run a new database call and display its results without having to reload the whole page. 

Most of the code has been chopped up and commented for help. All of the identifying information and keys have been removed - you'll need to add those on your own.

If you have any questions, feel free to contact me. 

Jeremy Riel
GE2 Technology Director
