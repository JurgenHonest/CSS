# CSS

CSS (Cascading Style Sheets) is a stylesheet language used to control the presentation and layout of HTML documents. It enables web developers to separate content (HTML) from design (CSS), allowing for more flexible and maintainable web pages. CSS defines how elements should be displayed on different devices by specifying styles such as colors, fonts, spacing, positioning, and responsiveness. 

## Selectors of CSS

Selectors in CSS are patterns used to select the elements you want to style. They are a fundamental part of CSS because they define which elements in the HTML document the styles will apply to. CSS selectors can range from very simple to quite complex, depending on how specific you need to be.

### 1. Universal Selector (*):
Selects all elements in the document.
Example
```
* {
  margin: 0;
  padding: 0;
}
```
This example resets the margin and padding for all elements.

### 2. Type Selector (Element Selector):

Selects all elements of a given type.
Example:
```
p {
  font-size: 16px;
}
```
Applies the font size to all <p> (paragraph) elements.

### 3. Class Selector (.):

Selects elements that have a specific class attribute.
Example:
```
.button {
  background-color: #3498db;
  color: white;
}
```
Targets all elements with the class "button".

### 4. ID Selector (#):

Selects an element with a specific id attribute. IDs should be unique within a page.
Example:
```
#header {
  background-color: #333;
  color: white;
}
```
Targets the element with the id "header".

### 5. Attribute Selector:

Selects elements based on an attribute or attribute value.
Examples:
```
input[type="text"] {
  width: 200px;
}
```

```a[target="_blank"] {
  color: red;
}
```

### 6. Child Selector (>):

Selects elements that are direct children of a specified element.
Example:
```
.menu > li {
  list-style-type: none;
}
```
Selects only the <li> elements that are direct children of the element with the class "menu".

### 7. Pseudo-Class Selectors (continued):
#### a. :hover:
Targets an element when a user hovers over it with a pointing device.
```
a:hover {
  color: #0056b3;
}
```
#### b. :nth-child(n): 
Selects elements based on their position among their siblings. The n can be a number, keyword, or formula.
```
li:nth-child(odd) {
  background-color: #f0f0f0;
}
```
This example selects all odd-numbered li elements.

#### c. :first-child:
Selects the first child of its parent.
```
p:first-child {
  font-weight: bold;
}
```
This targets the first p child of any parent.

#### d. :last-child: 
Selects the last child of its parent.
```
p:last-child {
  margin-bottom: 0;
}
```
This removes the bottom margin of the last p child

### e. :nth-of-type(n): 
Similar to :nth-child, but only counts siblings of the same type.
```
div:nth-of-type(2) {
  color: red;
}
```
This targets the second div of its parent.

### 8. Pseudo-Element Selectors:
Pseudo-elements target specific parts of an element or create elements dynamically.

#### a. ::before:
Inserts content before the content of an element.
```
.quote::before {
  content: "“";
  font-size: 2em;
  color: #ccc;
}
```
Adds a quotation mark before the content of elements with the class "quote".

#### b. ::after: Inserts content after the content of an element.
```
.quote::after {
  content: "”";
  font-size: 2em;
  color: #ccc;
}
```
Adds a closing quotation mark after the content of elements with the class "quote".

#### c. ::first-letter: 
Styles the first letter of the selected element.
```
p::first-letter {
  font-size: 2em;
  color: #3498db;
}
```
Enlarges and colors the first letter of each paragraph.

#### d. ::first-line: 
Styles the first line of text within the selected element.
```
p::first-line {
  font-weight: bold;
}
```
Makes the first line of each paragraph bold.

### 9. Group Selector (``, ):
Allows you to apply the same styles to multiple selectors.
Example:
```
h1, h2, h3 {
  font-family: 'Arial', sans-serif;
  color: #333;
}
```
This example applies the same font and color to all h1, h2, and h3 elements.















