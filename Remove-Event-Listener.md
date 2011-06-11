removeEventListener can be called on an 'eventTarget' if the event handler was added with [[addEventListener]] using a [[named function]] as opposed to a [[anonymous function]].

##Usage
    var namedCallbackFunction = function( eventObj ){
        // write code to respond to event in here
        // log eventObj to see the cool stuff on the event object
    }
    
    EventTarget
      .addEventListener('eventType', namedCallbackFunction, false);

    EventTarget
      .removeEventListener('eventType', namedCallbackFunction, false);

### Signature
    eventTarget.addEventListener('eventTarget', namedCallbackFunction, useCapture)

* ** eventTarget**: an object against which an event may be dispatched (eg: the window, document, an element, etc.)
* **type**: A string indicating the [[event|Events]] type to unbind from.
* **namedCallbackFunction**: The named function to be unbound from the eventTarget.
* **useCapture**: (optional) If true, useCapture specifies whether the EventListener being removed was registered as a capturing listener or not. If a listener was registered twice, one with capture and one without, each must be removed separately. Removal of a capturing listener does not affect a non-capturing version of the same listener, and vice versa.

