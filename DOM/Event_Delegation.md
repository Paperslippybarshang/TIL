# Event Delegation

Today, I learned about a programming concept called Event Delegation. It is a design pattern that allows us to listen for events on multiple elements just by setting up an event handler to a single parent element. So whenever an event is fired in any of the child nodes (or its children), the event handler will get executed even thought it was directly bound to the child nodes.

Here's an example:

```
<ul>
  <li>Item 1 <button type="submit"> Button 1 </button> </li>
  <li>Item 2 <button type="submit"> Button 2 </button> </li>
  <li>Item 3 <button type="submit"> Button 3 </button> </li>
</ul>
```

Let's say there's a `<button>` nested inside one of the `<li>` elements. If we wanted to listen for a 'click' event in Button 1, normally we would add an event listener to Button 1. However, the issue is that we would have to add event listener to each of the buttons. To avoid these repetition, we can simply add an event listener to a single parent element, which is `<ul>`. Then, once you `console.log(event.target)` and click any of its child nodes - `<li>` or `<button>` - you'll see that an event is fired even though the event handler is not directly attached to that targeted element.

For more information -> https://dmitripavlutin.com/javascript-event-delegation/
