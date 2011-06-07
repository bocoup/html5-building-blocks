The browser provides a powerful programming interface for traversing and manipulating the document. This is often called DOM traversal and manipulation. DOM stands for Document Object Model. This object representation of the `[[document]]` after it is loaded into the `[[window]]` provides numerous methods for interacting with itself, and stores numerous interesting properties about the current state of the `document. 

You can interact with the DOM through `document` and `element` methods and properties. Many of the DOM methods are polymorphic across `document` and `element` in that the same method name does different things depending on weather it is called on `document` or `element`.


##Document
The browser provides us with a programming interface to the `document` currently loaded into a `[[window]]`. See the [[methods reference | https://developer.mozilla.org/en/DOM/document#Methods]] and [[properties reference | https://developer.mozilla.org/en/DOM/document#Properties]] on MDC for a full list of all the properties and methods on the `document`.

To quickly see all of the properties and methods on the `document`, open up your [[JavaScript Console]], and type:

    window.document


##Element
