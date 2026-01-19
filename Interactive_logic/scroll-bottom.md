# Scroll to Bottom

Scrolls the viewport to the bottom of the page.
Uses the Window Scrolling API.

```js
<button onClick={()=>window.scrollTo({
        top:document.body.scrollHeight,
        behaviour:'smooth'
    }) }>
<button/>
```
### When to use
- Footer navigation (Contact, Support)
- Chat apps (auto-scroll)
- Lazy-loaded content
### Runs only in cilent side
