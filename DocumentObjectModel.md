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

## querySelector 

-The querySelector() method returns the first element that matches a specified CSS selector(s) in the document.

-Note: The querySelector() method only returns the first element that matches the specified selectors. To return all the matches, use the querySelectorAll() method instead.

-If the selector matches an ID in document that is used several times (Note that an "id" should be unique within a page and should not be used more than once), it returns the first matching element.

## innerText

-The innerText property can be used to write the dynamic text on the html document. Here, text will not be interpreted as html text but a normal text.

-It is used mostly in the web pages to generate the dynamic content such as writing the validation message, password strength etc.

-Syntax:

Return the text content of a node:
        node.innerText

Set the text content of a node:
        node.innerText = text

## innerHTML

-The innerHTML property sets or returns the HTML content (inner HTML) of an element.

Syntax:

Return the innerHTML property:
        HTMLElementObject.innerHTML

Set the innerHTML property:
        HTMLElementObject.innerHTML = text

## setAttriute

-The setAttribute() method adds the specified attribute to an element, and gives it the specified value.

-If the specified attribute already exists, only the value is set/changed.

-Note: Although it is possible to add the style attribute with a value to an element with this method, it is recommended that you use properties of the Style object instead for inline styling, because this will not overwrite other CSS properties that may be specified in the style attribute:

-Bad:
        element.setAttribute("style", "background-color: red;");

-Good:
        element.style.backgroundColor = "red";

-Example: add the class attribute with the value of "democlass" to a <h1> element:

        document.getElementsByTagName("H1")[0].setAttribute("class", "democlass");

## Style Property

-The style property returns a CSSStyleDeclaration object, which represents an element's style attribute.

-The style property is used to get or set a specific style of an element using different CSS properties.

***Note: It is not possible to set styles by assigning a string to the style property, e.g. element.style = "color: red;". To set the style of an element, append a "CSS" property to style and specify a value, like this:
        element.style.backgroundColor = "red";   // set the background color of an element to red

-As you can see, the JavaScript syntax for setting CSS properties is slightly different than CSS (backgroundColor instead of background-color).

-Example: add a red color to an <h1> element:

        document.getElementById("myH1").style.color = "red";

## classList Property.

-Example: add the "mystyle" class to a <div> element:

        document.getElementById("myDIV").classList.add("mystyle");

-The classList property returns the class name(s) of an element, as a DOMTokenList object.

-This property is useful to add, remove and toggle CSS classes on an element.

-The classList property is read-only, however, you can modify it by using the add() and remove() methods.