# Full-Stack-Interview-Practice
Full Stack Interview practice has some of interview questions that are related to job requirements. 

Interview questions

1. What is the most influential book or blog post you’ve read regarding web  development?
  - Well, I cannot really say it as a blog post or book but back in college, we had a brief introduction about HTML in our courses. I found it very interesting and tried to find about it in more detail. 
   When I typed about HTML in the google browser, the very first thing I found was w3schools.com.  I have researched the site and really enjoyed the resources regarding web development. 
   That was my first ever influential thing that happened and helped me to pursue web development.
  
2. Tell me about the web application you have built. Why did you choose to build it? What did you learn? What challenges did you face and how did you overcome them?
 -  I build a Restaurant Menu application as the part of the Full Stack nanodegree and hosted it on AWS server. The application basically shows the list of restaurants
    and their menus.
 - I have used Flask framework in this application,  learned about RESTful APIs that serve JSON and XML output, and front-end HTML/CSS/JS that renders the Restaurants and their Menus. In this application, I have also learned how the session and routing works.
   The challenges for me was when I started working with this application I had a minimal Knowledge of flask and SQLAlchemy database. So I had to explore about flask and SQLAlchemy,  One more challenge was to organize the code well and understand how the session works, as well as working with G+ Login. With the help of Udacity coaches and reading the recommended documentation about the flask and looking into the examples provided in the lessons, helped to understand and made this application possible.

3. Wite a function in Python that takes a list of strings and return a single string that is an HTML unordered list(<ul>….</ul>) of those strings. You should include a brief explanation of your code. Then, what would you have to consider  if the original list was provided by user input?
 
n = ['Micheal', 'Lorean']

def list(strings):  
    lst = '<ul>'
    /* Iteration over strings
    for s in strings:
        /* append the list items in the strings
        lst += '<li>%s</li>' % s
    /* append the closing of unordered list   
    lst += '</ul>'

    /* returns unorderedlist    
    return lst

print list(n);

If we give the user input for the list. It prints the unordered list with the list items.
Output : 
<ul>
<li>Micheal</li>
<li>Lordan</li>
</ul>

4. List 2-3 attacks that web applications are vulnerable to. How do these attacks work? How can we prevent those attacks?
  -	SQL injection attacks to gain access to the database, spoof  a user’s identity,  and destroy or alter data in the database. SQL injection occurs when malicious SQL statements are inserted into form fields to try and gather information from the database. This information enables the hacker to access, modify or destroy information in the database. With SQL injection a hacker can change the price of a product, and gain customer information such as credit card numbers, password and contact information.
  -	Distributed Denial of Service Attacks (DDoS). DDoS attacks generate requests from thousands  of IP addresses in an attempt to flood a site with traffic, making it impossible for the server to respond to requests. DDoS attacks or bots can slow a site down or make it temporarily unavailable.
  -	Cross Site Request Forgery (CSRF) attacks. CSRF attacks occur when a user is tricked into clicking a link or downloading an image that executes unwanted actions on an unauthenticated user session.
  
  Attack-specific solutions include:
  1. Implementing CAPTCHA or prompting users to answer questions. This ensures that a form or request is being submitted by a human and not a bot.
  2. Use a Web Application Firewall to monitor your network and block potential attacks.
 

