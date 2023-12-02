# JavaScript30 Notes

## Day 1：　JavaScript Drum Kit
- Custom data attributes (data-*) is used to store custom data private to the application. The stored (custom) data can then be used in the page's JavaScript to create a more engaging user experience.
- The querySelector() method returns the first element that matches a CSS selector. Otherwise null. QuerySelectorAll() can be used if theres multiple.  document.querySelector(".myclass") will give back the first element in the document with the class "myClass"
- document.querySelector("div.user-panel.main input[name='login']"); Here, the first input element with the name "login" (\<input name="login"/>) located inside a \<div> whose class is "user-panel main" (\<div class="user-panel main">) in the document is returned:
- TThe Element.classList is a read-only property that returns a live DOMTokenList collection of the class attributes of the element. .classList.add() is a method in JavaScript that adds one or more class names to the specified element. We also have .remove and .toggle. 

 ## Day 2: CSS + JS Clock
 The position property
 - Static positioned elements are not affected by the top, bottom, left, and right properties. An element with position: static; is not positioned in any special way; it is always positioned according to the normal flow of the page:
 - An element with position: relative; is positioned relative to its normal position. Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.
 - An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.
 - An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed). However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling. Note: Absolute positioned elements are removed from the normal flow, and can overlap elements.
 - An element with position: sticky; is positioned based on the user's scroll position. A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed).
 - If position: absolute; or position: fixed; - the left property sets the left edge of an element to a unit to the left of the left edge of its nearest positioned ancestor. If position: relative; - the left property sets the left edge of an element to a unit to the left/right of its normal position. If position: sticky; - the left property behaves like its position is relative when the element is inside the viewport, and like its position is fixed when it is outside. If position: static; - the left property has no effect.

 ## Day 3: Playigng with CSS Variables and JS
 - The :root selector matches the document's root element.
 - Custom properties are entities defined by CSS authors that represent specific values to be reused throughout a document. Custom property can be declared with a prefix of two dashes. 
 - The var() function is used to insert the value of a CSS variable.
 - dataset is an object that contains all the data attributes in the element. 
 - data-* attributes are custom attributes that can be added to HTML elements to store custom data.
 - setProperty(propertyName, value)
 - Document.documentElement returns the element that is the root element of the document (HTML element)
 - how to set CSS custom property. (document.documentElement.style.setProperty("--name", "value"))


 ## Day 4: Array Cardio Day 1
 - array.reduce(function(total, currentValue, currentIndex, arr), initialValue)
 - for sort(), if the returned value is 1, it means to place a after b [b,a]. If it is negative then b after a [a,b]. If 0, keep the original order. So -1, then keep the normal order of a before b. If the result is negative, a is sorted before b.
- you can run querySelector() in any existing DOM element. 
- The spread (...) syntax allows an iterable, such as an array or string, to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected

## Day 5: Flex Panels Image Gallery
- flex:1 makes sure that the elements will grow equally (extra space is distributed equally)
- element can both be flex items and flex container
- The :first-child pseudo class selector is used to select the specified selector, only if it is the first child of its parent. ul > :first-child means selecting the first child of ul element.  (https://www.w3schools.com/cssref/sel_firstchild.php)

## Day 6:　Ajax Type Ahead
- fetch() returns a promise. We need to call .then() against it. 
- fetch() gives you back raw data. (response object) blob.json() will return another promise. 
- (BLOB stands for Binary Large Object. It is defined as the chunk of binary data being stored as a single entity in a database system.)
- A Promise is an object representing the eventual completion or failure of an asynchronous operation. It is used to find out if the asynchronous operation succeeded or not. 
- spread syntax allows you to expand array into each element. (for example to put into an argument of a function which requires one element as one argument)  