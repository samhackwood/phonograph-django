![General Assembly's Logo](https://camo.githubusercontent.com/603ef5eae7d28900a9678ae96c6c60a9c72f8a059c328b28cf978df999cea1f8/68747470733a2f2f692e696d6775722e636f6d2f6c7a56493364382e706e67)

# The Phonograph - A Collection of Records

## Overview
![App home page screenshot](/thephonograph/main_app/static/images/Homepage%20Screenshot.png)
![Record detail page screenshot](/thephonograph/main_app/static/images/Record%20Detail%20Screenshot.png)


### Requirements
- The application includes at least 2 related models, one of them being the User, and the major CRUD functions have been implemented
- Some pages have a restricted access, therefore they can only be viewed by logged-in Users, the User is also able to sign-up/login, change the password and logout
- The Users receives feedback messages for success/fail form submissions, some of the forms have mandatory fields otherwise the User is not allowed to submit them; after every submission the forms are cleared of the data

### Technologies Used
- Git/GitHub
- HTML and CSS
- CSS Library
- Python
- Django
- PostgreSQL
- pgAdmin 4

### Team Members
- Elisabetta Maspero - [GitHub](https://github.com/emaspero) | [LinkedIn](https://www.linkedin.com/in/elisabetta-maspero-990bb3111/)
- Cristopher Carey - [GitHub](https://github.com/christopher-k-c) | [LinkedIn](https://www.linkedin.com/in/chriskcarey/)
- Sam Hackwood - [GitHub](https://github.com/samhackwood) | [LinkedIn](https://www.linkedin.com/in/samuel-hackwood-40b050233/)

### Process

Unfortunately, I had missed the previous week of classes due to having COVID and I was advised to catch up on recorded lectures before helping my group. So, I spent the first three days of the project teaching myself Django and chipping in with wireframes and user stories. Fortunately, having previously worked with Express, I knew all the same back-end principles that are at the heart of Django and I picked it up pretty easily. By day four my group was nearly finished with the project and all that was left to do was styling and deployment! I decided therefore that I would continue to work on the project after it was initially submitted so that I could get some real ‘hands-on’ experience with using Django and python. 

Having discussed with my group what added functionality could further develop the site, they suggested that a user profile where the user can edit, update, and delete their accounts would be useful. So, over the course of about, five days, in my spare time, I got to work on the user profile as well as fixing a few bugs here and there. To do this I used the Django user model to display user information, then created the appropriate URLs, HTML pages, and controllers to allow the user to update or delete their information. 


###### Trello
![Trello board screenshot picture](/thephonograph/main_app/static/images/Trello%20Screenshot.png)
[Trello Board](https://trello.com/b/NnHgZg5d/project-03)
###### ERD (Entity Relationship Diagrams)
![ERDs screenshot](/thephonograph/main_app/static/images/ERDs%20Screenshot.png)
###### Wireframes
![Figma screenshot](/thephonograph/main_app/static/images/Figma%20Screenshot.png)
###### User Stories
![User Stories](/thephonograph/main_app/static/images/User%20Stories.png)

## Challenges 

The most significant challenge for me during this process was having to go alone without help from my instructors or my team. To get through the project I had to hone my diagnostic skills when  things inevitably went wrong, as well as a lot of help from the Django documentation and Stack Overflow. Though this made the development process quite challenging for me, I began to grow in confidence quickly as I realised that all I needed was a bit of patience and I could solve the majority of issues myself. 

Another issue I faced was the limitation due to Django rails. Something that I wanted to implement for the user profile was a profile picture. I later realised however that this was not something that is available in the pre-build user model which Django provides. This meant that if I wanted to implement the profile picture, I would have to completely tear out everything I had done with the user model and start from scratch which would have been far too time consuming for what I wanted to achieve on the app. So, in the end I decided simply to put a placeholder image where the profile picture would be.



### Deployed application link
[The Phonograph](https://hydro-keener-88414.herokuapp.com/)
### Challenges
As a Team we did find it challenging to fully understand what happens in the background with the CBVs, as the code is a lot shorter and less obvious than express, it's not always immediate to fully comprehend and subsequently work with the code. We did struggle understanding how to pull the data from models that were linked by relationships and show it on the page (eg. how to display the Artist name from the Record page considering that the relationship was a many to many). We decided to implement a CSS Library that we did not use during the lectures before, Tailwind, and does take time and understanding to be able to fully make the best out of these kind of features. When debugging we did run a vast amount of Google searches and the answers that we get from the web are not always the easiest to understand/implement due to the wide amount of different ways in which developers work, especially based on their experience. 

### Features to be added in the future
- The password reset email only gets sent to the Terminal at the moment, the link fully works and the functionality fully works, but it would be good to have it as an actual sent email instead. As well, we could implement a verification email to be sent upon registration of a new User.
- Implement on the homepage a carousel showing the latest record that have been added to the database.
- Different levels of privileges based on the User type. 
- Make the app fully responsive.
- Install Tailwind with the config file, rather than just import it via the link, to fully explore how to personalize it.
- Embed Youtube video related to Artist/Record on the detail pages.
- Utilize a third party API, in this case Discogs API and include pagination. 
- Create a Label model that behaves in a similar way to the Artist model.
