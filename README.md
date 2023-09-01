### Character_Counter_js
# Hosted Link:-https://tulasidurga1.github.io/Character_Counter_js/
### Explanation:-
### HTML Structure:

## The HTML file starts with the usual <!DOCTYPE html> declaration and includes meta tags for character set, compatibility, and viewport settings.
The title of the web page is set as "Real-time Character Counter."
A custom CSS file ("style.css") is linked for styling.
The <body> contains a <div> with the class "container" to hold the main content.
## Inside the container:
An <h2> heading with the title "Real-time Character Counter."
A <textarea> element with the ID "textarea." This is where the user can input text.
The maxlength attribute is set to 50 characters.
A <div> with the class "counter-container" to hold the character count information.
Two <p> elements are inside this div to display the total characters and remaining characters.
Each <p> contains a <span> element with a class to display the actual counts.
CSS Styling (style.css):

## The CSS file defines styles for various elements on the page, such as the background color, container width, heading alignment, textarea dimensions, and counter font size.
JavaScript Implementation (index.js):

## The JavaScript code is placed at the bottom of the <body> and starts with three variable declarations:
textareaEl: References the textarea element.
totalCounterEl: References the span element for displaying the total character count.
remainingCounterEl: References the span element for displaying the remaining character count.
Event Listener and Function:

## An event listener is added to the textareaEl element for the "keyup" event. This means that whenever the user types or releases a key in the textarea, the function will be triggered.
The updateCounter function is defined. It is responsible for updating the character counters in real-time.
updateCounter Function:

## The updateCounter function calculates and updates the character count and remaining character count.
It updates the innerText property of totalCounterEl with the length of the value entered in the textarea.
It calculates the remaining characters by subtracting the current text length from the maxlength attribute of the textarea, and then updates the innerText of remainingCounterEl.
Initial Counter Update:

## The updateCounter function is called initially to set the counters based on any initial content in the textarea.
