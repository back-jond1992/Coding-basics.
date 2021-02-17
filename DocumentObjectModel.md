# DOM

-With the HTML DOM, JavaScript can access and change all the elements of an HTML document.

-When a web page is loaded, the browser creates a Document Object Model of the page.

-The HTML DOM model is constructed as a tree of Objects:

-With the object model, JavaScript gets all the power it needs to create dynamic HTML:
    .JavaScript can change all the HTML elements in the page
    .JavaScript can change all the HTML attributes in the   page
    .JavaScript can change all the CSS styles in the page
    .JavaScript can remove existing HTML elements and attributes
    .JavaScript can add new HTML elements and attributes
    .JavaScript can react to all existing HTML events in the page    
    .JavaScript can create new HTML events in the page

## What is the DOM?

-The DOM is a W3C (World Wide Web Consortium) standard.

=The DOM defines a standard for accessing documents:

"The W3C Document Object Model (DOM) is a platform and language-neutral interface that allows programs and scripts to dynamically access and update the content, structure, and style of a document."

-The W3C DOM standard is separated into 3 different parts:

    Core DOM - standard model for all document types
    XML DOM - standard model for XML documents
    HTML DOM - standard model for HTML documents

-The HTML DOM is a standard object model and programming interface for HTML. It defines:

    .The HTML elements as objects
    .The properties of all HTML elements
    .The methods to access all HTML elements
    .The events for all HTML elements

-In other words: The HTML DOM is a standard for how to get, change, add, or delete HTML elements.

## QuerySelector 

-The querySelector() method returns the first element that matches a specified CSS selector(s) in the document.

-Note: The querySelector() method only returns the first element that matches the specified selectors. To return all the matches, use the querySelectorAll() method instead.

-If the selector matches an ID in document that is used several times (Note that an "id" should be unique within a page and should not be used more than once), it returns the first matching element.

