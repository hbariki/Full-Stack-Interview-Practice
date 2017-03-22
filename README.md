# Full-Stack-Interview-Practice
Full Stack Interview practice has some of interview questions that are related to job requirements. 

Interview questions

1. What is the most influential book or blog post you’ve read regarding web  development?
  - Well, I cannot really say it as a blog post or book but back in college, we had a brief introduction about HTML in our courses. I found it very interesting and tried to find about it in more detail. 
   When I typed about HTML in the google browser, the very first thing I found was w3schools.com.  I have researched the site and really enjoyed the resources regarding web development. 
   That was my first ever influential thing that happened and helped me to pursue web development.
  
2. Tell me about the web application you have built. Why did you choose to build it? What did you learn? What challenges did you face and how did you overcome them?
 -  I build a Restaurant Menu application as the part of the Full Stack nanodegree and hosted it on AWS server. The application basically shows the list of restaurants and their menus, users can register through G+ Login. Registered users can create, edit, delete, update the restaurants and their menus.
 - I have used Flask framework in this application,  learned about RESTful APIs that serve JSON and XML output, and front-end HTML/CSS/JS that renders the Restaurants and their Menus. In this application, I have also learned how the session and routing works.
   The challenges for me when working on this project was when I started working with this application I had a minimal Knowledge of flask and SQLite database. So I had to explore about flask and SQLite, Another challenge was to organize the code well and understand how the session works, as well as working with G+ Login. With the help of Udacity coaches and reading the recommended documentation about the flask and looking into the examples provided in the lessons, helped to understand and made this application possible.As per the job description it includes that we should have knowledge about the technologies like Python, dijango, javascript. I have worked with Flask in couple of projects, Now I can understand the basic things how to work with a web framework. I am sure that If an opportunity is provided, I will be able to work with django within short period of time.I am comfortable working with Javascript. I have build a project called Neighborhood Map with Knockout.js, jQuery, bootstrap, CSS, HTML. The application bascially displays the map with markers, shows the nearby 
restaurants in San Francisco.   

3. Wite a function in Python that takes a list of strings and return a single string that is an HTML unordered list(<ul>….</ul>) of those strings. You should include a brief explanation of your code. Then, what would you have to consider  if the original list was provided by user input?
``` 
def list(strings):
  lst = '<ul>'
  # Iteration over strings
  for s in strings:
    # append the list items in the strings
    lst += '<li>%s</li>' %s
    # append the closing unordered list
  lst += '</ul>'
    # returns unordered list
  return lst
 
  ``` 
  If the original list is supplied by user input, the function should check if the input is a list, and if the list contains strings.

4. List 2-3 attacks that web applications are vulnerable to. How do these attacks work? How can we prevent those attacks?
  -	SQL injection attacks to gain access to the database, spoof  a user’s identity,  and destroy or alter data in the database. SQL injection occurs when malicious SQL statements are inserted into form fields to try and gather information from the database. This information enables the hacker to access, modify or destroy information in the database. With SQL injection a hacker can change the price of a product, and gain customer information such as credit card numbers, password and contact information.
  -	Distributed Denial of Service Attacks (DDoS). DDoS attacks generate requests from thousands  of IP addresses in an attempt to flood a site with traffic, making it impossible for the server to respond to requests. DDoS attacks or bots can slow a site down or make it temporarily unavailable.
  -	Cross Site Request Forgery (CSRF) attacks. CSRF attacks occur when a user is tricked into clicking a link or downloading an image that executes unwanted actions on an unauthenticated user session.
  
  Attack-specific solutions include:
  -Implementing CAPTCHA or prompting users to answer questions. This ensures that a form or request is being submitted by a human and not a bot.
  - Use a Web Application Firewall to monitor your network and block potential attacks.
  - The best practices that can be used on an ongoing basis to protect your application and users are Code reviews, bug bounty programs      and code scanners should be implemented throughout the application lifecycle. Code reviews can help spot vulnerable code early in          development phase, dynamic and static code scanners can do automatic checks for vulnerabilities, and bug bounty programs enable            professional pen testers to find bugs in the website.
 
5. Here is some starter code for a Flask Web Application. Expand on that and include a route that simulates rolling two dice and returns    the result in JSON. You should include a brief explanation of your code.
```
from flask import Flask
app = Flask(__name__)

import json
import random

@app.route('/)
def hello_world():
  return 'Hello world!'
  
@app.route('/roll_dice/<int:sides>/json')
def roll_dice(sides):
    #Return the result of two dice with user specified number of sides being rolled as a json object
    
    # Assign the result of the die roll
    die1 = random.randint(1, sides)
    die2 = random.randint(1, sides)
    
    # Return the results of the dice rolled as JSON string, sorted by key
    return json.dumps({'die1' :die1 , 'die2':die2}, sort_keys = True)

if __name__ == '__main__':
 app.debug = True
 app.run()
```
6. If you were to start your full-stack developer position today, what would be your goals a year from If now?

-I would like to be part of an environment that promotes learning and professional career growth. 
-While progressing through the nanodegree program along with Python using Flask framework I worked on couple of the projects. Besides, I have  also started learning Node.js, I developed an Employee application using Node.js, Angular.js, postgresSQL. It displays the details of the employees and users will be able to create, update, delete, edit the details.
- For the next 12 months I am looking forward to learn django, explore flask and Node.js in more detail.
- As a medical industry is a vast industry, I have always been very curious to learn about the gentics and also new techniques which are     related to medical industry. It would be an exciting opportunity for me. If opportunity is provided I would like to know more about this   in detail as well.  

References:
- http://stackoverflow.com/questions/33069476/simulating-rolling-2-dice-in-python
- https://www.instartlogic.com/blog/4-common-web-application-security-attacks-and-what-you-can-do-prevent-them

