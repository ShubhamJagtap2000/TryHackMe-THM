# Task 6 - Cookies

You've probably heard of cookies before, they're just a small piece of data that is stored on your computer. 

Cookies are saved when you receive a "Set-Cookie" header from a web server. 

Then every further request you make, you'll send the cookie data back to the web server. 

Because HTTP is stateless (doesn't keep track of your previous requests), cookies can be used to remind the web server who you are, some personal settings for the website or whether you've been to the website before. 

Let's take a look at this as an example HTTP request:
    
   ![Screenshot (750)](https://user-images.githubusercontent.com/63872951/178449549-42c8cd51-67e3-4690-b776-e495972e26da.png)


Cookies can be used for many purposes but are most commonly used for website authentication. 

The cookie value won't usually be a clear-text string where you can see the password, but a token (unique secret code that isn't easily humanly guessable).

# Answer the questions below

1. Which header is used to save cookies to your computer?
```
Set-Cookie
```
