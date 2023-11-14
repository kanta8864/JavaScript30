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
