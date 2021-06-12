#  Object 
 **An object** is a collection of  __properties__, and a property is an association between a name (or key) and a value. A property's value can be a function, in which case the property is known as **a method**.

# DOM (Document Object Model)
In the **DOM**, all HTML elements are defined as **objects**.

The programming interface is the properties and methods of each object.

+  A **property** is a value that you can get or set (like changing the content of an HTML element).

![obj](https://fireship.io/courses/javascript/img/js-object-props.png)


+  A **method** is an action you can do (like add or deleting an HTML element).

![dom](https://miro.medium.com/max/1120/0*dcpjTwj_qSjTdaUc.jpg)

# Finding HTML Elements
	
| Method |  Description |
| ------------ | -------------|
|document.getElementById(id) |	Find an element by element id |
|document.getElementsByTagName(name) |	Find elements by tag name |
|document.getElementsByClassName(name) |	Find elements by class name |

# Changing HTML Elements

| Method |  Description |
| ------------ | -------------|
|element.innerHTML =  new html content |	Change the inner HTML of an element
|element.attribute = new value| Change the attribute value of an HTML element|
|element.style.property = new style	|Change the style of an HTML element
|**Method**	|**Description**|
|element.setAttribute(attribute, value)	| Change the attribute value of an HTML element| 

# Adding and Deleting Elements
| Method |  Description |
| ------------ | -------------|
|document.createElement(element)|	Create an HTML element|
|document.removeChild(element) |	Remove an HTML element|
|document.appendChild(element) |	Add an HTML element |
|document.replaceChild(new, old) |	Replace an HTML element |
|document.write(text)	| Write into the HTML output stream |