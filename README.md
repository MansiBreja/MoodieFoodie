# MoodieFoodie
*...Food for every Mood*

This is a web application which recommends you food based on your mood using machine learning and delivers it to your doorstep.

We understand that the first thought that comes to our mind when we come across a food suggesting and delivery app, is obviously- "HOW IS THIS SOMETHING NEW?"

We'll explain.
This web application is based on an absolutely new idea and is completely different from the traditional food delivery websites.

Firstly, it suggests a list of restaurants combining three basic parameters i.e cost, user rating and distance, all at the same time. Hence, it offers you the most optimal choice available, saving you the trouble of choosing the best restaurant for you using individual filters on traditional apps. 
The most commonly used apps allow you to choose a restaurant on the basis of only a single critera at a time, but we recommend you the nearest, most affordable and best quality restaurants, thereby catering to all your demands at the same time without having you to compromise on any of them.

Secondly, we understand that there are times when you are unable to decide what to order. Infact, we have personally faced this dilemma a hundred times when we've spent hours scrolling a food delivery app, thinking about the most important question which seems to have been given the least importance uptil now , "WHAT TO EAT?" 
MoodieFoodie helps you to choose a food item for all your moods, be it a happie, a sadie, an angrie, a dehydratie, a depressie, an excitie or an unwellie mood ;")
Whatever be your mood, we can always suggest you food!

The app uses previous user moods and their respective food orders to suggest the best food choice for you.

Thirdly, we offer several other options for food ordering like the list of food items ordered the most at a particular time of the day or the restaurants that can order food in the minimum time if you're really hungry or the top searched food items, etc.

And lastly, this app allows you to order the food items that traditional food delivery apps don't.
You can order tea, juices or even chocolates. For this, we have a separate "Wanna sell on MoodieFoodie" option for small scale sellers like small tea shops, women who make homemade chocolates or other small scale setups who wish to sell online.

## Working and Implementation
<ul>
<li>The major feature of our project which sets it apart from the traditional apps of its kind needs three parameters to order the list of recommended restaurants with the highly recommended restaurant at the top. These three features are the user ratings, cost for two people and the restaurant's distance from the user.
<ul>
<li>Whenever any user orders from a certain restaurant, he/she is asked to rate the restaurant out of 5. The rating of that restaurant is then dynamically updated using the mathematical average of the current rating and the new rating. This computation also requires the storage of the number of ratings for a particular restaurant.
<li>The cost for two people is permanently stored initially when a restaurant is added to the database.
<li>To compute the distance of the user from a restaurant, we have stored the geocode of all the restaurants in the database. We have used the Google Maps API to extract the user's geocode and hence compute his/her distance.</li>
</ul>
A very simple model of machine learning, that is logistic regression is used to implement the same. When the user chooses a certain restaurant among the recommended restaurants, then his/her choice to select a certain restaurant and discard other restaurants is used to train the model which only increases the accuracy of the algorithm.
<li>The USP of our project, which is recommending the users food items based on their mood works on previous users' inputs only. Whenever any user orders from a certain restaurant, he/she is asked to specify what his/her mood was before he/she had ordered. His/Her order and mood is used to train the algorithm which gradually increases its accuracy.
<li>To help small businesses expand their reach by selling on our application, we have simply provided them with a form wherein they can fill out the necessary details.
</ul>

## Installation Requirements

```
Framework : Django, Version : 1.11.17
Language : Python, Version : 3.6.3

To run it, you need to install some packages and libraries as follows:
Bootstrap 3
numpy
sklearn
bcrypt
django[argon]

Install dependencies directly from requirements.txt in pip installation,
To install these, write this on the command line terminal:
"pip install -r requirements.txt"
```

## To run

```
Clone this repo
cd into this repo
Enter command: "pip install -r requirements.txt"
Enter the command: "python manage.py runserver"
Copy the url and paste it in your favourite browser window.
```

## See for youself:

![screenshot 15](https://user-images.githubusercontent.com/31369977/38465883-bbfb3816-3b3e-11e8-9f3d-183e0700e477.png)
![screenshot 40](https://user-images.githubusercontent.com/31369977/38466463-18b83fe2-3b47-11e8-91bc-e1763d4d4ece.png)
![screenshot 16](https://user-images.githubusercontent.com/31369977/38465884-bc297fc8-3b3e-11e8-9384-c481358b8bfa.png)
![screenshot 18](https://user-images.githubusercontent.com/31369977/38465886-bc8cf3e6-3b3e-11e8-9451-583b8854a3a7.png)
![screenshot 19](https://user-images.githubusercontent.com/31369977/38465887-bcbca942-3b3e-11e8-9528-77e8cefbff29.png)
![screenshot 20](https://user-images.githubusercontent.com/31369977/38465888-bcee7120-3b3e-11e8-87e7-2b8eaa811638.png)
![screenshot 32](https://user-images.githubusercontent.com/31369977/38466417-516fe1d8-3b46-11e8-82ba-7a1cd22c4622.png)
![screenshot 39](https://user-images.githubusercontent.com/31369977/38466416-5144b878-3b46-11e8-8da1-b2523d93d95e.png)
![screenshot 31](https://user-images.githubusercontent.com/31369977/38465882-bbcf2df2-3b3e-11e8-9192-60f4dbe03276.png)

This project was made collectively by [Mansi Breja](https://github.com/MansiBreja), [Kavita Maurya](https://github.com/Kavita309) and [Anjali Agarwal](https://github.com/aganjali10) as a part of the HackBMU Hackathon, BML University, Gurgaon, Haryana. 
