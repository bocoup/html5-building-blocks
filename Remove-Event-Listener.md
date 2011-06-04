removeEventListener can be called on an EventTarget if the event handler was added with [[addEventListener]] using a [[named function]] as opposed to a [[anonymous function]].

##Usage
    var listener = function( eventObj ){
        // write code to respond to event in here
        // log eventObj to see the cool stuff on the event object
    }
    
    EventTarget
      .addEventListener('eventType', listener, false);

    EventTarget
      .removeEventListener('eventType', listener, false);

### Signature
    EventTarget.removeEventListener('eventType', callbackFunction, useCapture)

* ** EventTarget**: an object against which an event may be dispatched (eg: the window, document, and html element, etc.)
* **type**: A string representing the event type to listen for.
* **callbackFunction**: The object that receives a notification when an event of the specified type occurs. This must be an object implementing the EventListener interface, or simply a JavaScript function.
* **useCapture**: (optional) If true, useCapture indicates that the user wishes to initiate capture. After initiating capture, all events of the specified type will be dispatched to the registered listener before being dispatched to any EventTargets beneath it in the DOM tree. Events which are bubbling upward through the tree will not trigger a listener designated to use capture. See DOM Level 3 Events for a detailed explanation. Note that this parameter is not optional in all browser versions.
