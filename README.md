# Sprint-Challenge Applied Javascript - Lambda Times

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored the DOM and the concept of components. During this Sprint, you studied the DOM, DOM Events, and Components. In your challenge this week, you will demonstrate proficiency by creating an online Lambda newspaper called "Lambda Times."

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in Applied JavaScript.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.

## Description

You are going to create a Lambda Newspaper. Your job is going to be to add functionality to the tabs below the 'Lambda Times' logo. These tabs will act as filters for our articles, and when clicked on, should filter out all articles except those with that tag.

![Working Sprint Challenge Gif](./Sprint-Challenge.gif 'Example of working project')

In meeting the minimum viable product (MVP) specifications listed below, you should have a console full of correct responses to the problems given.

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1. What is the DOM?
The DOM is an API that represents the entire webpage, with all it's content, structure and styling. The DOM gives us the ability to manipulate the document of the webpage _without_ actually mutating the underlying `.html`-file. For example, with JavaScript, we can identify different elements in the browser and then modify them to achieve a certain goal. The DOM is tree-shaped, following the structure of the HTML document. As such, the 'highest' element will always be `document`, followed by the root element, which is `<html>`.

2. What is an event?
An event is the denotation we use to signifiy that something has happened or changed within the browser. One of the foremost examples of an event would be the webpage loading on the user's browser. As soon as all files are received from the servers and correctly implemented, an event 'fires' with all relevant data attached to it. Other examples would be a button getting clicked, a mouse moving over a specific element or resizing the browser window. In effect, whenever something 'happens' or 'changes' on the webpage (even when it might not be obvious to the user), an event fires.
Often, when an event is intentionally triggered, you may want to do something as a result, which leads us to...

3. What is an event listener?
An event listener is a method that's added to a specific browser element. The method accepts two parameters; a event or event-specifier and a function that's to be executed as soon as the specified event fires on the designated element. There are dozens of different events you can use as a parameter and you can inject whatever function you desire. Finally, there's also no limit to how many eventListeners you can add to a single element. The function passed to the `.addEventListener()`-method can also do anything and everything you want it to do, within the parameters of JavaScript. At it's core, `.addEventListener()`is responsible for the vast majority of interactivity we see on the web nowadays.

4. Why would we convert a NodeList into an Array?
The DOM uses nodes and elements to keep track of the entire webpage. When we select a collection of web elements - let's say all the `<button>` elements - we get a NodeList containing all the relevant items. A NodeList looks rather similar to an Array at first glance. However, its prototype is different, which means that its functionality is dissimilar as well. To use all the array methods we've come to love (and occassionally hate), we need to transform the NodeList into an array. This can be done by using `Array.from(${NodeList})`.

5. What is a component?
Components are building blocks used in making our website. When using similar elements in more than place in a website, it makes sense to isolate and standardize that piece of code - let's say for a `<button>` or an element with class `.productCard`. In doing so, we'd make a single element, style it correctly and make sure it has the correct functionality, and then simply reuse this newly-made component wherever necessary, with some slight alterations if need be. Components are an incredibly powerful way to build webpages, large and small, and allows for rapid prototyping. It's much easier to slap a dozen pre-existing components together than hand-writing every single element and style indicator for an entire page. Bootstrap is well-known for it's incredibly versatile library of components.

### Git Set up

* [x] Fork the project into your GitHub user account
* [x] Clone the forked project into a directory on your machine
* [x] Create a pull request before you start working on the project requirements.  You will continuously push your updates throughout the project.
* [x] You are now ready to build this project with your preferred IDE

## Minimum Viable Product

Your finished project must include all of the following requirements:

* [ ] Look through the HTML code paying particular attention to the Tabs component and the Cards components. You will notice they share a data attribute. We will be using this data attribute to determine which cards should show when each tab is selected.

* [ ] Following the instructions in the `Tabs.js` file, complete the `TabLink`, and `TabCard` class components. It will look and feel very similar to the last project we worked on, but with a twist. Now, instead of one `Item` to display, we will need to display a collection of `Cards`. Think about ways to iterate over an array and manipulate each item.  **Note: You will need to un-comment the code after the lines of instructions.  The code is commented out so you can work error-free**

* [ ] Once you get your `Tab` component working properly add a couple more articles yourself and check out how it works.

## Stretch Problems

Your stretch challenge is to write the functionality of a `Carousel` component. You have the HTML and CSS already in place, simply un-comment the HTML in the `index.html` file. This is an advanced challenge, so you are not expected to be able to complete it. If you begin and don't finish, you should still submit with what you have. You may reference the `Tabs.js` file for assistance.

* [ ] Complete the carousel functionality in `Carousel.js`

* [ ] If you complete the Carousel, add functionality so that the carousel slides when the buttons are pressed instead of just appearing.

* [ ] Create an 'infinite loop' carousel. In which as long as you click on an arrow, the array of images will loop over itself.

* [ ] If you have finished the above, play around with the styling on all the components, and understand how each is built.
