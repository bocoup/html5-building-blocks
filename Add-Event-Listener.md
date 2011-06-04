##Usage
    EventTarget
      .addEventListener('eventType', function( eventObj ){
        // write code to respond to event in here
        // log eventObj to see the cool stuff on the event object
      }, false);
### Signature
    EventTarget.addEventListener('eventType', callbackFunction, useCapture)

* ** EventTarget**: an object against which an event may be dispatched (eg: the window, document, and html element, etc.)
* **type**: A string representing the event type to listen for.
* **callbackFunction**: The object that receives a notification when an event of the specified type occurs. This must be an object implementing the EventListener interface, or simply a JavaScript function.
* **useCapture**: (optional) If true, useCapture indicates that the user wishes to initiate capture. After initiating capture, all events of the specified type will be dispatched to the registered listener before being dispatched to any EventTargets beneath it in the DOM tree. Events which are bubbling upward through the tree will not trigger a listener designated to use capture. See DOM Level 3 Events for a detailed explanation. Note that this parameter is not optional in all browser versions.

##Every Event Type:
###[[Mouse Events]]
####[[click]]
Fires when the pointing device button is clicked over an element. A click is defined as a mousedown and mouseup over the same screen location. The sequence of these 

####[[dblclick]]
Fires when the pointing device button is [[double click]]ed over an element

####[[mousedown]]
Fires when the pointing device button is pressed over an element

####[[mouseup]]
Fires when the pointing device button is released over an element

####[[mouseover]]
Fires when the pointing device is moved onto an element

####[[mousemove]]
Fires when the pointing device is moved while it is over an element

####[[mouseout]]
Fires when the pointing device is moved away from an element

####[[drag]] 
Fires when a draggable element is dragged.

####[[drop]]
Fires when a draggable element is dropped.

###[[Keyboard Events]]
####[[keydown]]
Fires before keypress, when a key on the keyboard is pressed.

####[[keypress]]
Fires after keydown, when a key on the keyboard is pressed. 

####[[keyup]]
Fires when a key on the keyboard is released.

###[[Navigation Events]]
####[[hashchange]]
Fires when the location hash changes.

####[[popstate]]
Fires when the history object is updated.

###[[Window Events]]
####[[message]]
Fired on the window when a message is received from from another context.

####[[load]]
Fires when the window finishes loading all content within a document, including window, frames, objects and images. For elements, it fires when the target element and all of its content has finished loading.

####[[unload]]
Fires when the user agent removes all content from a window or frame. For elements, it fires when the target element or any of its content has been removed.

####[[abort]]
Fires when an object/image is stopped from loading before completely loaded.

####[[error]]
Fires when an object/image/frame cannot be loaded properly.

####[[resize]]
Fires when a document view is resized.

####[[scroll]]
Fires when a document view is scrolled.

###[[Form Events]]
####[[select]]
Fires when a user selects some text in a text field or textarea.

####[[change]]
Fires when a control loses the input focus and its value has been modified since gaining focus.

####[[submit]]
Fires when a form is submitted.

####[[reset]]
Fires when a form is reset.

####[[focus]]
Fires when an element receives focus either via the pointing device or by tab navigation.

####[[blur]]
Fires when an element loses focus either via the pointing device or by tabbing navigation.

###[[Touch Events]]
####[[touchstart]]
Fires when a finger is placed on the touch surface/screen.

####[[touchend]]
Fires when a finger is removed from the touch surface/screen.

####[[touchmove]]
Fires when a finger already placed on the screen is moved across the screen.

####[[touchenter]]
Fires when a touch point moves onto the interactive area defined by a DOM element.

####[[touchleave]]
Fires when a touch point moves off the interactive area defined by a DOM element.

####[[touchcancel]]
Fires when a TouchPoint has been disrupted in an implementation-specific manner, such as by moving outside the bounds of the window, or if more touch points are activated than supported by the implementation.

###[[User Interface Events]]
####[[DOMFocusIn]]
Similar to HTML focus event, but can be applied to any focusable element.

####[[DOMFocusOut]]
Similar to HTML blur event, but can be applied to any focusable element.

####[[DOMActivate]]
Fires when an element is activated, for instance, through a mouse click or a keypress.

###[[Mutation Events]]
####[[DOMSubtreeModified]]
Fires when the subtree is modified.

####[[DOMNodeInserted]]
Fires when a node has been added as a child of another node

####[[DOMNodeRemoved]]
Fires when a node has been removed from a DOM-tree

####[[DOMNodeRemovedFromDocument]]
Fires when a node is being removed from a document

####[[DOMNodeInsertedIntoDocument]]
Fires when a node is being inserted into a document

####[[DOMAttrModified]]
Fires when an attribute has been modified

####[[DOMCharacterDataModified]]
Fires when the character data has been modified

###[[Media Events]]