Events added with addEventListener can be removed later using [[removeEventListener|Remove Event Listener]] if the event handler is added using a [[named function]] as opposed to a [[anonymous function]].

##Usage
###anonymous function
    eventTarget
      .addEventListener('eventType', function( eventObj ){
        // write code to respond to event in here
        // log eventObj to see the cool stuff on the event object
      }, false);

###named function
    var listener = function( eventObj ){
        // write code to respond to event in here
        // log eventObj to see the cool stuff on the event object
    };
    eventTarget
      .addEventListener('eventType', listener, false);

### Signature
    eventTarget.addEventListener('eventTarget', callbackFunction, useCapture)

* ** eventTarget**: an object against which an event may be dispatched (eg: the window, document, an element, etc.)
* **type**: A string indicating the [[event|Events]] type to listen for.
* **callbackFunction**: The function to be called when the given event is fired on the eventTarget. This function takes an [[Event Object]] as an optional argument.
* **useCapture**: (optional) If true, useCapture indicates that the user wishes to initiate capture. After initiating capture, all events of the specified type will be dispatched to the registered listener before being dispatched to any EventTargets beneath it in the DOM tree. Events which are bubbling upward through the tree will not trigger a listener designated to use capture. See DOM Level 3 Events for a detailed explanation. Note that this parameter is not optional in all browser versions.