# Halfway Hackathon

**Congratulations!** Today we are at the halfway point in our class. Let's celebrate with a hackathon! A hackathon is a great opportunity to work on a larger, real-world project, while reviewing and solidifying the core concepts that we've covered in the first half of the course.

## Step 1: Make a Plan

1. Take a few minutes to brainstorm some project ideas. This could be related to your community site, a stand-alone project, or just a crazy mash-up site to help you practice different coding concepts
2. Review the Step 3: Coding section below to consider the different concepts that we hope to practice during this project.
3. In your group, hold a standup meeting to present your plan of what you'd like to accomplish, and potential stumbling blocks.
4. If someone mentions being concerned about a concept that you feel solid on, offer to be a resource for them if they have questions.

------

## Step 2: Set up a GitHub repo

1. Open the **Terminal** and run:
```
git config --global user.name "YOUR NAME"
git config --global user.email "YOUR EMAIL ADDRESS"
```

2. Go to [GitHub](https://github.com/) and sign in or sign up for an account.
3. Create a new repository on GitHub by clicking the new repository menu, upper-right.
4. Follow the instructions presented in the new repository.

>If you'd like to know more about the philosophy behind version control, check out The Git Parable

-----

## Step 3: Coding

The following lists the core web development skills that you should feel comfortable using in your project thus far:

1. Using Markdown to create a README.md file introducing your project.
2. Pushing to GitHub and seeing it rendered on your repository's main page.
3. Creating an HTML document using the following HTML tags:
  + ```<html>```, ```<head>```, ```<title>```, ```<body>```
  + header and paragraph tags
  + bold and italic tags
  + ```<div>``` and ```<span>```
  + ordered and unordered lists
  + images and links
  + horizontal rule and line break
4. Using a style attribute on an HTML element, then a ```<style>``` tag in the head, then a ```<link>``` tag to a separate ```.css``` document to include CSS styles in your page. Try to use the following CSS properties at a minimum:
  + ```color, background-color, background-image```
  + ```font-size, font-family```
  + ```height, width, max-width```
  + ```margin, padding, border, border-radius```
5. Refactoring your code to use classes and ids.
6. Using some complex CSS selectors, like descendent selectors
7. Using an ```iframe``` to embed videos or maps on your page
8. Using ```float``` and and ```position:fixed``` to position some elements
9. Creating an HTML form incorporating various inputs (```text, password, email, textarea, radio, checkbox, select menu, submit```, etc)
10. Making your form live using Formspree
11. Using the Bootstrap grid system to lay out your page
12. Using some pre-written Bootstrap CSS classes on various elements of your page
13. Using ```alert```, ```prompt```, and ```console.log``` where appropriate
14. Setting and retrieving values from JavaScript variables
15. Using ```document.querySelector``` in conjunction with ```textContent``` and ```innerHTML``` to retrieve and place content on the page
16. Using ```if```, ```elseif``` and ```else``` to implement branching logic on the basis of comparing variables and values
17. Using logical and (```&&```), logical or (```||```), and the ternary operator
18. Using ```while``` loops to do work multiple times until a condition is met
19. Using the ```Math``` object and ```parseInt()```.
20. Using jQuery to select existing HTML elements on the page
21. Use jQuery's ```.css()```, ```.attr()```, ```.text()```, ```.html()```, ```.append()```, and ```.val()``` to both get and set values
22. Use some jQuery effects like ```.show()```, ```.slideDown()``` and ```.fadeOut()```

#### Stretch Goals:

1. Use some of Bootstrap's JavaScript utilities
2. Try incorporating some jQuery Plug-ins

------------

## Step 4: Deploy & Promote

1. Deploy your code to Divshot using your command line tools
2. Post a link on Slack
3. Send it to your friends and family members so they can be proud of you
4. Social media?

----------

## Step 5: Profit?

+ Monetize
+ Monetize
+ Monetize

-------

## A note regarding best practices:

Try to decipher the code below. What does it do?

```javascript
var i = 1, n = 5, j
while (i <= n){
j = 1;
var msg = '';
if (i === 1) {
msg += 'Welcome ' + i;
} else if (i > 1) {
msg += 'Welcome ' + i + ', meet';
}
while (j < n) {
if( j > 0 && j < i) {
if (j === i - 1) {
if (j === 1) {
msg += ' ' + j;
} else {
msg += ' and ' + j;
}
} else {
if (j === 1 && i === 3){
msg += ' ' + j;
} else {
msg += ' ' + j +',';
}
}
}
console.log(msg)
j++;
}
```
Pretty tough right? Here are some problems:

+ No indentation
+ Obscure variable names
+ A bit verbose

What happens when we clean it up?

```javascript
var guest_number, announcement_message, arrival_number = 1, total_number_of_guests = 5

while (arrival_number <= total_number_of_guests){
  guest_number = 1, announcement_message = 'Welcome ' + arrival_number

  if (arrival_number > 1) {
    announcement_message += ', meet ' + guest_number

    while (++guest_number < arrival_number ) {
      if (guest_number !== arrival_number - 1) {
        announcement_message += ', ' + guest_number
      } else {
        announcement_message += ' and ' + guest_number
      }
    }
  }
  arrival_number++
  console.log(announcement_message)
}
```
### Go and build something, with pretty code!
