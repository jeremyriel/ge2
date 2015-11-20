ge2 - A script codebase repository for the GlobalEd 2 curriculum
===
GlobalEd 2 (GE2, www.globaled2.com) is an online/in-person hybrid curriculum for middle school social studies. It focuses on the development of student interest, confidence and argumentation skills related to social studies and science by integrating science and social studies together. Students interact in an online negotiations simulation to solve a real-world socioscientific problem, such as global fresh water shortage or international food scarcity. 

Technology is a critical component of the types of activities that students do in GE2. Students perform significant research on the problem they are provided and collaboratively develop solutions with other middle school students in other schools. Students interact in an online simulation environment, which facilitates a multi-classroom learning experience. Students play the role of science advisors from an assigned country. They apply their research and develop arguments for proposals to the given problem scenario. At the conclusion of the negotiations, students sponsor proposals from other countries. 

To assist with students' research, members of the curriculum research and development staff have developed a few scripts to help with students' learning. 

# List of scripts
1. **A script with an interactive map of the world.** Students are assigned a country and interact with other countries in the negotiations simulation. They have to perform significant research to make sound arguments for proposals. We developed an interactive map of the countries represented in GE2 that displays relevant information from the CIA World Factbook. Students can get key statistics and links on their country, as well as other countries in the simulation. The map purposefully reduces the number of countries down to only those particpating in the simulation (i.e., the total number of classrooms participating) in order to reduce the complexity of students' initial research. This helps them have a "starting point" for their research, instead of the entire world of countries to consider all at once. 
  - Developed Summer 2014
  - Included in folder /map

2. **A script for managing the Knack database application and API.** I used the Knack database application (www.knackhq.com) to develop a "starting point" database of web resources for students using the curriculum. The curriculum staff wanted a list that was easily populated on multiple sites and with different formats, while only having to enter a resource into the database just once. A database was the way to go, and Knack provides an API that allows for multi-site connection. In addition, Knack provides the hosting and bandwidth for the database. I had to custom-write some scripts to get it to work for us, though. Since our websites run on Wordpress, I wanted something that could integrate well. I developed scripts in PHP to access the Knack API and parse the results. I also added filtering functionality so students could filter results by category. To do this, I used an AJAX call to repopulate the page's results whenever a new filter was applied without reloading the entire HTML. This script might be useful for people who want to use Knack to develop a database of their own to display a list of resources. Of couse, I have removed the API keys and such, and anyone wanting to customize the code will need to create new categories and fields. I tried to mark up the snippets and explain what is happening as well, as the Knack API documentation didn't reveal everything and was new to me as someone who was new to working with web services and HTTP requests.

# Thank you
Thank you for stopping by. Hopefully others can find some use in what we've built for students. I will keep adding things as we develop them. Please remember that our material is open to use and adapt, but please cite us and our project if you do. 

If you have any questions, feel free to contact me!

Jeremy Riel
GlobalEd 2 Technology Director
www.globaled2.com
