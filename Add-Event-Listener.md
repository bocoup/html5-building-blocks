##Usage
object.addEventListener('eventType', callbackFunction, useCapture)
eg:
    
    object
      .addEventListener('eventType', function( eventObj ){
        // write code to respond to event in here
        // log eventObj to see the cool stuff on the event object
      }, false);
* type: A string representing the event type to listen for.
* callbackFunction: The object that receives a notification when an event of the specified type occurs. This must be an object implementing the EventListener interface, or simply a JavaScript function.
* useCapture: (optional) If true, useCapture indicates that the user wishes to initiate capture. After initiating capture, all events of the specified type will be dispatched to the registered listener before being dispatched to any EventTargets beneath it in the DOM tree. Events which are bubbling upward through the tree will not trigger a listener designated to use capture. See DOM Level 3 Events for a detailed explanation. Note that this parameter is not optional in all browser versions.

##Every Event Type