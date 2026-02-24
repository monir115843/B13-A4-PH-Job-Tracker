Answers to Questions:

1. What is the difference between getElementById, getElementsByClassName, and querySelector/querySelectorAll?

-->getElementById: Selects a single element by its unique ID. It is highly efficient and returns only one element.

-->getElementsByClassName: Selects all elements with a specific class name and returns an 'HTMLCollection' (array-like object).

-->querySelector: Uses CSS selectors to find and return the first matching element. It is very flexible as it can select by ID, class, or tag.

-->querySelectorAll: Uses CSS selectors to find all matching elements and returns them as a 'NodeList'.

2. How do you create and insert a new element into the DOM?

-->To create a new element, use document.createElement('tagName').

-->To add content to the element, use .innerText or .innerHTML.

-->To insert the element into the DOM, use methods like appendChild() (adds as the last child) or prepend() (adds as the first child) on a parent element.

3. What is Event Bubbling? And how does it work?

Event Bubbling is a process where an event starts from the specific element that was triggered (the target/child) and then propagates up through its parent elements in the DOM tree. For example, if you click a button inside a div, the click event first triggers on the button and then moves up to the div.

4. What is Event Delegation in JavaScript? Why is it useful?

Event Delegation is a technique where you attach a single event listener to a parent element instead of adding multiple listeners to individual child elements.

-->Why it's useful: It is efficient for memory management. More importantly, it allows you to handle events for dynamically added elements (elements created after the page loads) without needing to attach new listeners to them.

5. What is the difference between preventDefault() and stopPropagation() methods?

-->preventDefault(): It cancels the default behavior of an element. For instance, it prevents a link from navigating to another URL or a form from refreshing the page upon submission.

-->stopPropagation(): It stops the event from bubbling up the DOM tree. This ensures that the event does not trigger any event listeners on the parent elements.