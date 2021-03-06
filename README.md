# Recipes Online

Recipes online is a member and non-member friendly website in which users can search for recipes 
which other users have shared. 

Every user will have the option to register or not, when registered a profile will be created. 
This profile will show all the recipes the user has uploaded as well as showing recipes they have 
favourited for later use.

## **Members can:**
* Log into their profile at any time. 
* Share recipes that will be available to everyone. 
* Favourite recipes to make them easier to locate at a later date. 
* Edit their own recipes.
* Delete their recipes from the site at any time.
* Search the recipes using the search bar. 

## **Non-Members can:**
* View any recipe which members have shared.
* Search the recipes using the search bar. 

# UX 
This website is for novice to advanced bakers/cooks, who want a community to share recipes and try new 
recipes. 
My website will help them achieve this as they are able to make a profile if they want to, and have a profile
page where the recipes they have added are stored, and where they can favourite recipes for later use. 

## User Stories

* As a member and non-member, I want a search bar to make searching for specific recipes easier. 
* As a new user to the wesbite, I want an option to register to make a profile to save my recipes. 
* As a member, I want to be able to add new recipes to my profile.
* As a member, I want to be able to favourite recipes so they are easier to find at a later daye. 
* As a member, I want the option to edit the recipes I have uploaded to the site.
* As a member, I want the option to delete the recipes I have uploaded to the site. 

# Features

* **The register feature:**
This gives all visitors to the website the option to register 
to the website and benefit from all the listed features above. 
* **The login feature:**
Once registered, users can login to their profile. When logged in
they can 'add a new recipe', 'edit' and 'delete' recipes that they 
have added. They will also be able to 'favourite' any recipes 
on the website. 
* **Add a new recipe:**
This is a faeture that is only available to registered users.
They can store any recipes they wish too. The recipe will then be available 
for anyone to see (both registered and unregistered).
* **Edit recipe:**
This feature will only be available to the specific user that created the recipe. 
They will be able to edit any recipe they have addded to the site in case they made 
a mistake. 
* **Delete recipe:**
This is feature that will only be available to the user that added the recipe. 
If they decide then want to delete the recipe from the site they are able too with 
this function. 
* **Favourite recipe:**
Registered users are able to favourite any recipe that is on the site. 
This recipe will then be added to a personalized 'favourites' page. 
* **Remove from favourites:**
If the user no longer wants the favourite recipe on their favourites page,
they will be given the option to remove it from the page. 
* **Search bar:**
This allows user and non-users to search specific words within the website to help find recipes faster. 

# Technologies Used
Within the website, I have used many external resources to help construct the webiste and 
increased the user experience. 
### Jquery 
A widely known external library to 'write less, do more'. It simplifies the code needed when
using Javascript. https://jquery.com/
### Materialize
A framework to style the layout of the website and make it mobile responsive. 
https://materializecss.com/
### Font Awesome
This is an external library of icons which have been used around the site to make it more
visually appealing. 
https://fontawesome.com/icons?d=gallery

# Testing 

### Python code checker
Throughout the project, I used https://extendsclass.com/python-tester.html to check the python code 
and syntax was all correct, and made any changes accordingly. 

### Search bar 
To test the search bar function, I used a word I knew was in the recipes list and made sure it showed up.
I then used a word I knew wasn't in the recipes list and made sure the 'no recipes found' messsage
appeared. 

### Register function 
To test the register function:
* Go to the register page to make sure it connects correctly.
* Enter a username without a password to make sure an error occurs and that an account is not 
made.
* Enter a username that I knew was already in use to make sure that an error occurs which says; "username
already in use"
* Enter a valid username and password, which should successfully make a profile.
* If a profile has been made more options on the nav bar should appear. I.e 'add recipe',
'view favourites', 'profile'. 

### Log In function
To test the log in function:
* Go to log in page to make sure it connects properly. 
* Enter and incorrect username and/or password to make sure an error occurs which says; "incorrecr 
username and/or password"
* Enter correct username and password, which should successfully log user in. 
* If user has been logged in more options on the nav bar should appear. I.e 'add recipe',
'view favourites', 'profile'.

### Add new recipes
When the user is logged in they should be able to add new recipes when they click on the 'Add new recipe'
button on the nav bar. 
To test this, I added a recipe and made sure that the recipe was correctly added to the home page, 
profile page and to mongo DB.

### Edit recipes
* The edit button is formatted only to show up on recipes that the logged in user can see. To test this 
I added a recipe on one users profile and made sure that the edit button appeared. I then logged out 
and logged back in as a different user to test the edit button did not show on their profile. 

* When the edit button is clicked the user is re-directed to a new page to edit the recipe. 
On this page, the form is auto-filled with the correct recipe that has been selecetd, to test this 
I made multiple recipes and clicked edit on all of them. 
Once I had edited the recipe and clicked 'submit', I checked on the recipes page that they recipe
has been changed and also checked on mongo DB to make sure that it had been updated also. 

### Delete recipes
As with the edit recipes, the delete recipes button was also formatted only to show up on recipes that
the logged in user can see. To test this I added a recipe on one users profile and made sure that the delete button appeared. I then logged out 
and logged back in as a different user to test the delete button did not show on their profile. 

To test the delete function, I had to delete a recipe and make sure it was deleted completely of the 
website and also deleted from mongoDB. 

### Add to favourites 
The add to favourites function is something that is only available to registered users. 
To test the add to favourites function, I logged in and selected the 'add to favourites' on multiple
recipes to test that it; redirected to the favourites.html page and added the recipe to the page. 

### Delete from favourites
If the user favourites a recipe and then later on decides they no longer want that recipe on their 
favourites page, they are given the option to remove it from the page. 
To test this function, I added multiple recipes to favourites and then removed them to make sure that
the flash message worked and that the recipe was removed. 

# Deployment 
To deploy my app I have used heroku, which is then automatically connected to github. 
Everytime I pushed my work git, it automatically deployed to heroku. I made sure to push my work 
regularly in order to make sure I did not lose any work and that it was all up-to-date. 
The website can be found at: https://recipes-online-cr.herokuapp.com/


