The browser provides a powerful programming interface for traversing and manipulating the document. This is often called DOM traversal and manipulation. DOM stands for Document Object Model. This object representation of the document after it is loaded into the window provides numerous methods for interacting with itself. You can interact with the DOM through `document` and `element` methods properties. Many of the DOM methods are polymorphic across `document` and `element` in that the same method name does different things depending on weather it is called on `document` or `element`.


##Document
###Properties
###Methods

##Element
###Properties
* [[attributes]]:  All attributes associated with an element.
* [[baseURI]]:  Base URI as a string
* [[baseURIObject New in Firefox 3]]:  The read-only nsIURI object representing the base URI for the element.
* [[childElementCount New in Firefox 3.5]]:  The number of child nodes that are elements.
* [[childNodes]]:  All child nodes of an element.
* [[children Requires Gecko 1.9]]:  A live nsIDOMNodeList of the current child elements.
* [[classList Requires Gecko 1.9.2]]:  Token list of class attribute
* [[className]]:  Gets/sets the class of the element.
* [[clientHeight]]:  The inner height of an element.
* [[clientLeft]]:  The width of the left border of an element.
* [[clientTop]]:  The width of the top border of an element.
* [[clientWidth]]:  The inner width of an element.
* [[contentEditable Requires Gecko 1.9]]:  Gets/sets whether or not the element is editable.
* [[dataset]]:  Allows access to read and write custom data attributes on the element.
* [[dir]]:  Gets/sets the directionality of the element.
* [[firstChild]]:  The first direct child node of an element, or null if this element has no child nodes.
* [[firstElementChild Requires Gecko 1.9]]:  The first direct child element of an element, or null if the element has no child elements.
* [[id]]:  Gets/sets the id of the element.
* [[innerHTML]]:  Gets/sets the markup and content of the element.
* [[isContentEditable Requires Gecko 2]]:  Indicates whether or not the content of the element can be edited. Read only.
* [[lang]]:  Gets/sets the language of an element's attributes, text, and element contents.
* [[lastChild]]:  The last direct child node of an element, or null if this element has no child nodes.
* [[lastElementChild Requires Gecko 1.9]]:  The last direct child element of an element, or null if the element has no child elements.
* [[localName]]:  The local part of the qualified name of an element. In Firefox 3.5 and earlier, the property upper-cases the local name for HTML elements (but not XHTML elements). In later versions, this does not happen, so the property is in lower case for both HTML and XHTML. Requires Gecko 1.9.2
* [[name]]:  Gets/sets the name attribute of an element.
* [[namespaceURI]]:  The namespace URI of this node, or null if it is no namespace. In Firefox 3.5 and earlier, HTML elements are in no namespace. In later versions, HTML elements are in the http://www.w3.org/1999/xhtml namespace in both HTML and XML trees. Requires Gecko 1.9.2
* [[nextSibling]]:  The node immediately following the given one in the tree, or null if there is no sibling node.
* [[nextElementSibling New in Firefox 3.5]]:  The element immediately following the given one in the tree, or null if there's no sibling node.
* [[nodeName]]:  The name of the node.
* [[nodePrincipal New in Firefox 3]]:  The node's principal.
* [[nodeType]]:  A number representing the type of the node. Is always equal to 1 for DOM elements.
* [[nodeValue]]:  The value of the node. Is always equal to null for DOM elements.
* [[offsetHeight]]:  The height of an element, relative to the layout.
* [[offsetLeft]]:  The distance from this element's left border to its offsetParent's left border.
* [[offsetParent]]:  The element from which all offset calculations are currently computed.
* [[offsetTop]]:  The distance from this element's top border to its offsetParent's top border.
* [[offsetWidth]]:  The width of an element, relative to the layout.
* [[ownerDocument]]:  The document that this node is in, or null if the node is not inside of one.
* [[parentNode]]:  The parent element of this node, or null if the node is not inside of a DOM Document.
* [[prefix]]:  The namespace prefix of the node, or null if no prefix is specified.
* [[previousSibling]]:  The node immediately preceding the given one in the tree, or null if there is no sibling node.
* [[previousElementSibling New in Firefox 3.5]]:  The element immediately preceding the given one in the tree, or null if there is no sibling element.
* [[schemaTypeInfo]]:  Returns TypeInfo regarding schema information for the element (also available on Attr).
* [[scrollHeight]]:  The scroll view height of an element.
* [[scrollLeft]]:  Gets/sets the left scroll offset of an element.
* [[scrollTop]]:  Gets/sets the top scroll offset of an element.
* [[scrollWidth]]:  The scroll view width of an element.
* [[spellcheck]]:  Controls spell-checking (present on all HTML elements)
* [[style]]:  An object representing the declarations of an element's style attributes.
* [[tabIndex]]:  Gets/sets the position of the element in the tabbing order.
* [[tagName]]:  The name of the tag for the given element.
* [[textContent]]:  Gets/sets the textual contents of an element and all its descendants.
* [[title]]:  A string that appears in a popup box when mouse is over the element.


###Methods
* [[addEventListener( type, listener, useCapture )]]: Register an event handler to a specific event type on the element.
* [[appendChild( appendedNode )]]: Insert a node as the last child node of this element.
* [[blur()]]: Removes keyboard focus from the current element.
* [[click()]]: Simulates a click on the current element.
* [[cloneNode( deep )]]: Clone a node, and optionally, all of its contents.
* [[compareDocumentPosition ( otherNode )]]: dispatchEvent( event )]]: Dispatch an event to this node in the DOM.
* [[focus()]]: Gives keyboard focus to the current element.
* [[getAttribute( name )]]: Retrieve the value of the named attribute from the current node.
* [[getAttributeNS( namespace, name )]]: Retrieve the value of the attribute with the specified name and namespace, from the current node.
* [[getAttributeNode( name )]]: Retrieve the node representation of the named attribute from the current node.
* [[getAttributeNodeNS( namespace, name )]]: Retrieve the node representation of the attribute with the specified name and namespace, from the current node.
* [[getBoundingClientRect ( )]]: getClientRects ( )]]: Returns a collection of rectangles that indicate the bounding rectangles for each line of text in a client.
* [[getElementsByClassName ( )]]: getElementsByTagName( name )]]: Retrieve a set of all descendant elements, of a particular tag name, from the current element.
* [[getElementsByTagNameNS( namespace, name )]]: Retrieve a set of all descendant elements, of a particular tag name and namespace, from the current element.
* [[getFeature ( feature, version  )]]: getUserData ( key )]]: hasAttribute( name )]]: Check if the element has the specified attribute, or not.
* [[hasAttributeNS( namespace, name )]]: Check if the element has the specified attribute, in the specified namespace, or not.
* [[hasAttributes()]]: Check if the element has any attributes, or not.
* [[hasChildNodes()]]: Check if the element has any child nodes, or not.
* [[insertBefore( insertedNode, adjacentNode )]]: Inserts the first node before the second, child, Node in the DOM.
* [[isDefaultNamespace ( namespaceURI )]]: isEqualNode ( nodeArg )]]: isSameNode ( otherNode ) 
* [[isSupported ( feature, version )]]: lookupNamespaceURI ( prefix )]]: lookupPrefix ( namespaceURI )]]: mozMatchesSelector( selector )]]: Returns whether or not the element would be selected by the specified selector string.
* [[normalize()]]: Clean up all the text nodes under this element (merge adjacent, remove empty).
* [[querySelector( selectors[, nsresolver] ) New in Firefox 3.5
* [[querySelectorAll( selectors[, nsresolver] ) New in Firefox 3.5
* [[removeAttribute( name )]]: Remove the named attribute from the current node.
* [[removeAttributeNS( namespace, name )]]: Remove the attribute with the specified name and namespace, from the current node.
* [[Name & Description
* [[removeAttributeNode( attrNode )]]: Remove the node representation of the named attribute from the current node.
* [[removeChild( removedNode )]]: Removes a child node from the current element.
* [[removeEventListener( type, handler, useCapture )]]: Removes an event listener from the element.
* [[replaceChild( insertedNode, replacedNode )]]: Replaces one child node in the current element with another.
* [[scrollIntoView( alignWithTop )]]: Scrolls the page until the element gets into the view.
* [[setAttribute( name, value )]]: Set the value of the named attribute from the current node.
* [[setAttributeNS( namespace, name, value )]]: Set the value of the attribute with the specified name and namespace, from the current node.
* [[setAttributeNode( name, attrNode )]]: Set the node representation of the named attribute from the current node.
* [[setAttributeNodeNS( namespace, name, attrNode )]]: Set the node representation of the attribute with the specified name and namespace, from the current node.
* [[setCapture( retargetToElement )]]: Sets up mouse event capture, redirecting all mouse events to this element.
* [[setIdAttribute (name, isIdBoolean)]]: Sets the attribute to be treated as an ID type attribute.
* [[setIdAttributeNS ( namespaceURI, localName, isIdBoolean )]]: Sets the attribute to be treated as an ID type attribute.
* [[setIdAttributeNode ( idAttr, isIdBoolean )]]: Sets the attribute to be treated as an ID type attribute.
* [[setUserData ( key, data, handler )]]





getElementById
getElementsByClassName
getElementsByTagName

createElement
appendChild

element.innerHTML
element.style.left
element.setAttribute
element.getAttribute
element.addEventListener
window.content
window.onload
window.dump
window.scrollTo

firstChild
lastChild
previousSibling
nextSibling
childNodes
