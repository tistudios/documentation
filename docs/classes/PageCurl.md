**super**: **[UIPageViewController](UIPageViewController.md)** (on iOS)

A page curl lets the user navigate between pages of content, where each page is managed by its own <a href="Window.html">Window</a> object. Navigation can be controlled programmatically by your app or directly by the user using gestures. When navigating from page to page, it displays a page-turning animation. The vertical style is not simulated in the Creo simulator for Mac

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **WillShow**()
Use this event to be notified when navigation is about to be added to a view hierarchy.

* **DidShow**()
Use this event to be notified when navigation was added to a view hierarchy.

* **WillHide**()
Use this event to be notified when navigation is about to be removed from a view hierarchy.

* **DidHide**()
Use this event to be notified when navigation was removed from a view hierarchy.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **bounds**: **[Rect](Rect.md)**
The bounds rectangle, which describes the view’s location and size in its own coordinate system.

* **var** **frame**: **[Rect](Rect.md)**
The frame rectangle, which describes the view’s location and size in its superview’s coordinate system.

* **var** **statusBarVisibility**: **StatusBarVisibility**
A value indicating whether the status bar should be visible.

* **var** **statusBarStyle**: **StatusBarStyle**
The style of the status bar.

* **var** **windows**: **[List](../gravity/list.md)**
Array of windows currently managed by the navigation.

* **var** **selectedWindow**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**
Represents the current Window in the navigation.

* **var** **selectedIndex**: **[Int](../gravity/types.md)**
Represents the current window index inside the navigation.



### Methods

* **func** **open**(**completion**: **[Closure](../gravity/closure.md) = null**)
Open window in currently displayed window or navigation using the destination object default behaviour.

* **func** **openIn**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **completion**: **[Closure](../gravity/closure.md) = null**)
<pre><code class="swift">TargetWindow.openIn(ContainerWindow);</code></pre>
Open callee object (TargetWindow) inside parameter object (ContainerWindow) using its default behaviour. Note that TargetWindow and/or ContainerWindow can be a Window or a Navigation.

* **func** **openWindow**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **completion**: **[Closure](../gravity/closure.md) = null**)
Add the Window to the PageCurl and set it as the selected Window.

* **func** **selectWindow**(**window**: **[Window](Window.md) or [NavigationBar](NavigationBar.md)**, **animated**: **[Bool](../gravity/types.md) = true**, **completion**: **[Closure](../gravity/closure.md) = null**)
Set the Window as the new selected Window, optionally animating the curl transition (this animation in not simulated in the Creo simulator for Mac).

* **func** **selectIndex**(**index**: **[Int](../gravity/types.md)**, **animated**: **[Bool](../gravity/types.md) = true**, **completion**: **[Closure](../gravity/closure.md) = null**)
Set the Window at the specified index as the new selected Window, optionally animating the curl transition (this animation in not simulated in the Creo simulator for Mac).

* **func** **openModal**(**TransitionStyle**: **<a href="#_enum_TransitionStyle">TransitionStyle</a>**, **completion**: **[Closure](../gravity/closure.md) = null**)
Open window modally usign the specified transition style.

* **func** **close**()
Close window if modally opened.





### Enumeration

#### StatusBarVisibility
 * .Default
 * .Hidden
 * .Visible

#### StatusBarStyle
 * .DarkContent
 * .Default
 * .LightContent

#### TransitionStyle
 * .Cards
 * .CoverVertical
 * .CrossDissolve
 * .Crossfade
 * .Cube
 * .Default
 * .Explode
 * .Flip
 * .FlipHorizontal
 * .Fold
 * .NatGeo
 * .NotAnimated
 * .PartialCurl
 * .Portal
 * .Turn



