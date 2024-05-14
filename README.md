D09
🧩 The Document Object Model

🧩 The Document Object Model
Completion requirements

The Document Object Model (The DOM)
Overview
The DOM is a representation of the HTML document in the browser. It allows us to interact with the page using JavaScript, modifying, adding and removing elements and text, images or other content.

Class Plan
Demo: Demonstration of the DOM and how it works
Workshop: Write some DOM manipulation code
Topics
What is the DOM?
How to access elements in the DOM
How to modify elements in the DOM
How to add elements to the DOM
How to remove elements from the DOM
Resources
MDN: The DOM
MDN: DOM manipulation
Workshop
Accessing elements
⛳️ In a new index.html file, add a script tag containing a console.log. Open the file in your browser and check the console to see the output.

console.log("Hello world!");
 
⛳️ Select the body element using the document.querySelector method. Log the element to the console.

const body = document.querySelector("body");

console.log(body);
 
⛳️ Select the h1 element using the document.querySelector method. Log the element to the console.

const h1 = document.querySelector("h1");

console.log(h1);
 
Modifying elements
You can modify elements in the DOM in various ways. The simplest is by setting the elements textContent property.

const h1 = document.querySelector("h1");

h1.textContent = "Hello world!";
 
Or updating the path to an image.

const image = document.querySelector("img");

image.src = "/images/myimage.jpg";
 
Adding elements
⛳️ Use the document object's document.createElement method to create a new header element and add it to the body with the body.appendChild method. In the browser, it will appear just as if you'd written the h1 in the file.

const body = document.querySelector("body");

const h1 = document.createElement("h1");
h1.textContent = "This is a heading!";
body.appendChild(h1);
 
🎯 Try to create a list of items by first creating a list, and then adding some list items to it. Finally, add the list to the body.

Removing elements
⛳️ Use the document object's document.querySelector method to select the h1 element and remove it from the DOM using the remove method.

const h1 = document.querySelector("h1");

h1.remove();
Your answer
