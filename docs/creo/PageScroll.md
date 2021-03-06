A `PageScroll` provides a way to implement linear navigation between pages of content, such as in a document, book, notepad, or calendar. A scrolling transition has no specific appearance; pages fluidly scroll from one to the next.

![PageScroll](../images/creo/PageScroll_main.png)

### Best practices
When a `PageCurl` or `PageScroll` is used, pages flow sequentially and there’s no way to jump between nonadjacent pages. If people may need to access pages out of sequence in your app, implement a custom control that provides this functionality.

### How to use
1. Drop a `PageScroll` 
2. Use the `PageScroll Inspector` to customize its scrolling direction (`Style`)

![PageScroll inspector](../images/creo/PageScroll_inspector.png)
The inspector where the `PageSroll` class can be configured.

### Example
- Start adding a `PageScroll` by tapping the _New Navigation_ button on the _bottom bar_

![New Navigation](../images/creo/PageScroll1.png)

- Configure the `Style` property from the inspector
- Create the `PageCurl` hierarchy by adding `Window` child screens
- For each `Window` set a different background color
- Repeat until you have a hierarchy like this

```
- PageScroll (startup window)
 - Window1
 - Window2
 - Window3
```

- Tap _Play_ and test the page scroll transition according to the `Style` property by swiping from right to left or from bottom to top.

### Most important properties
Several UI aspects can be configured in the `PageCurl` class but `Style` is the most important
- `Style`: is the scrolling direction, horizontal or vertical

### References
[PageScroll class reference](../classes/PageScroll.html) contains a complete list of properties and methods that can be used to customize a `PageScroll` object.
