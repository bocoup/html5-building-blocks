The browser provides a powerful programming interface for traversing and manipulating the document. This is often called DOM traversal and manipulation. DOM stands for Document Object Model. This object representation of the document after it is loaded into the window provides numerous methods for interacting with itself. You can interact with the DOM through `document` and `element` methods properties. Many of the DOM methods are polymorphic across `document` and `element` in that the same method name does different things depending on weather it is called on `document` or `element`.


##Document
###Properties
* [[document.activeElement]]: Returns the currently focused element
* [[document.alinkColor* Deprecated]]: Returns or sets the color of active links in the document body.
* [[document.all Deprecated]]:  
* [[document.anchors*]]: Returns a list of all of the anchors in the document.
* [[document.applets* Deprecated]]: Returns an ordered list of the applets within a document.
* [[document.async]]: async is used with document.load to indicate an asynchronous request.
* [[Node.attributes]]: Returns a collection of attributes of the given element
* [[document.background* Deprecated]]: Is supposed to return the URI of the image that tiles the background (though not apparently working in Mozilla); deprecated in favor of document.body.background (though HTML 4.01 deprecated this too)
* [[Node.baseURI]]: baseURI gets the base URI for the document
* [[document.baseURIObject Requires Gecko 1.9]]: baseURIObject returns an nsIURI object representing the base URI for the document.
* [[document.bgColor* Deprecated]]: Gets/sets the background color of the current document.
* [[document.body*]]: Returns the BODY node of the current document.
* [[document.characterSet]]: Returns the character set being used by the document.
* [[Node.childNodes]]: returns a collection of child nodes of the given node
* [[document.compatMode]]: Indicates whether the document is rendered in Quirks or Strict mode.
* [[document.contentType Non-standard
* [[Returns the Content-Type from the MIME Header of the current document.
* [[document.cookie*]]: Returns a semicolon-separated list of the cookies for that document or sets a single cookie.
* [[document.currentScript Requires Gecko 2.0 Non-standard]]: Returns the <script> element that is currently executing.
* [[document.defaultView]]: Returns a reference to the window object.
* [[document.designMode]]: Gets/sets WYSYWIG editing capability of Midas. It can only be used for HTML documents.
* [[document.dir ]]: Gets/sets directionality (rtl/ltr) of the document
* [[document.doctype]]: Returns the Document Type Definition (DTD) of the current document.
* [[Name]]: Description
* [[document.documentElement]]: Returns the Element that is a direct child of document. For HTML documents, this is normally the HTML element.
* [[document.documentURI]]: Returns the document location.
* [[document.documentURIObject Requires Gecko 1.9]]: Returns the nsIURI object representing the URI of the document. This property only has special meaning in privileged JavaScript code (with UniversalXPConnect privileges).
* [[document.domain*]]: Returns the domain of the current document.
* [[document.embeds]]: Returns a list of the embedded OBJECTS within the current document.
* [[document.fgColor* Deprecated]]: Gets/sets the foreground color, or text color, of the current document.
* [[document.fileSize]]: Returns size of the document or <img> element.
* [[Node.firstChild]]: Returns the first node in the list of direct children of the document.
* [[document.forms*]]: Returns a list of the FORM elements within the current document.
* [[document.height Unimplemented]]: Gets/sets the height of the current document.
* [[document.images*]]: Returns a list of the images in the current document.
* [[document.implementation]]: Returns the DOM implementation associated with the current document.
* [[document.inputEncoding]]: Returns the encoding used when the document was parsed.
* [[Node.lastChild]]: Returns the last child of a node
* [[document.lastModified]]: Returns the date on which the document was last modified.
* [[document.lastStyleSheetSet Requires Gecko 1.9]]: Returns the name of the style sheet set that was last enabled. Has the value null until the style sheet is changed by setting the value of selectedStyleSheetSet.
* [[document.linkColor* Deprecated]]: Gets/sets the color of hyperlinks in the document.
* [[Name]]: Description
* [[document.links*]]: Returns a list of all the hyperlinks in the document.
* [[Node.localName]]: Returns the local part of the qualified name of this node (null for a document)
* [[document.location]]: Returns the URI of the current document.
* [[document.mozCurrentStateObject Non-standard Requires Gecko 2.0]]: Returns the history entry at the top of the history stack without popping it off the stack. This also lets you look at the state without waiting for the popstate event to fire.
* [[Node.namespaceURI]]: Returns the XML namespace of the current document.
* [[Node.nextSibling]]: Returns the node immediately following the specified one in its parent's childNodes list, or null if the specified node is the last node in that list (null for documents)
* [[Node.nodeName]]: Returns the node's name (#document for document)
* [[Node.nodeType]]: Returns a node type constant (9 for document)
* [[Node.nodeValue]]: Returns the node's value (null for document)
* [[Node.nodePrincipal Requires Gecko 1.9]]: Returns the nsIPrincipal object representing current security context of the document.
* [[Node.ownerDocument]]: Returns the top-level document object for this node (null if already is the document).
* [[Node.parentNode]]: Returns the parent of the specified node in the DOM tree (null for document)
* [[document.plugins]]: Returns a list of the available plugins.
* [[document.popupNode]]: Returns the node upon which a popup was invoked (XUL documents only).
* [[document.preferredStyleSheetSet]]: Returns the preferred style sheet set as specified by the page author.
* [[Node.prefix]]: Returns the namespace prefix of the specified node, or null if no prefix is specified
* [[Node.previousSibling]]: Returns the node immediately preceding the specified one in its parent's childNodes list, null if the specified node is the first in that list (null for document)
* [[document.readyState Requires Gecko 1.9.2]]: Returns loading status of the document
* [[document.referrer*]]: Returns the URI of the page that linked to this page.
* [[document.selectedStyleSheetSet Requires Gecko 1.9]]: Returns which style sheet set is currently in use.
* [[document.styleSheets]]: Returns a list of the stylesheet objects on the current document.
* [[document.styleSheetSets Requires Gecko 1.9]]: Returns a list of the style sheet sets available on the document.
* [[Node.textContent]]: Returns null (returns other values for other nodes).
* [[document.title*]]: Returns the title of the current document.
* [[document.tooltipNode]]: Returns the node which is the target of the current tooltip.
* [[document.URL*]]: Returns a string containing the URL of the current document.
* [[document.vlinkColor* Deprecated]]: Gets/sets the color of visited hyperlinks.
* [[document.width Unimplemented]]: Returns the width of the current document.
* [[document.xmlEncoding]]: Returns the encoding as determined by the XML declaration.
* [[document.xmlStandalone]]: Returns true if the XML declaration specifies the document is standalone (e.g., An external part of the DTD affects the document's content), else false.
* [[document.xmlVersion]]: Returns the version number as specified in the XML declaration or "1.0" if the declaration is absent.

###Methods
* [[document.addEventListener]]: Adds an event listener to the document.
* [[document.adoptNode]]: Adopt node from an external document
* [[Node.appendChild]]: Adds a node to the end of the list of children of a specified parent node.
* [[document.captureEvents]]
* [[document.clear* Deprecated]]: In majority of modern browsers, including recent versions of Firefox and Internet Explorer, this method does nothing.
* [[Node.cloneNode]]: Makes a copy of a node or document
* [[document.close*]]: Closes a document stream for writing.
* [[Node.compareDocumentPosition]]: Compares the position of the current node against another node in any other document.
* [[document.createAttribute]]: Creates a new attribute node and returns it.
* [[document.createAttributeNS]]: Creates a new attribute node in a given namespace and returns it.
* [[document.createCDATASection]]: Creates a new CDATA node and returns it.
* [[document.createComment]]: Creates a new comment node and returns it.
* [[document.createDocumentFragment]]: Creates a new document fragment.
* [[document.createElement]]: Creates a new element with the given tag name.
* [[document.createElementNS]]: Creates a new element with the given tag name and namespace URI.
* [[document.createEntityReference]]: Creates a new entity reference object and returns it.
* [[document.createEvent]]: Creates an event.
* [[document.createExpression]]: Compiles an XPathExpression which can then be used for (repeated) evaluations. 
* [[document.createNSResolver]]: Creates an XPathNSResolver.
* [[document.createProcessingInstruction]]: Creates a new processing instruction element and returns it.
* [[document.createRange]]: Creates a Range object.
* [[document.createTextNode]]: Creates a text node.
* [[document.createTreeWalker]]: Creates a TreeWalker object.
* [[document.elementFromPoint]]: Returns the element visible at the specified coordinates.
* [[document.enableStyleSheetsForSet]]: Enables the style sheets for the specified style sheet set.
* [[document.evaluate]]: Evaluates an XPath expression.
* [[document.execCommand*]]: Executes a Midas command.
* [[document.execCommandShowHelp]]
* [[document.getBoxObjectFor]]
* [[document.getElementById]]: Returns an object reference to the identified element.
* [[document.getElementsByClassName]]: Returns a list of elements with the given class name.
* [[document.getElementsByName*]]: Returns a list of elements with the given name.
* [[document.getElementsByTagName]]: Returns a list of elements with the given tag name.
* [[document.getElementsByTagNameNS]]: Returns a list of elements with the given tag name and namespace.  
* [[Node.getFeature]]: document.getSelection
* [[Node.getUserData]]: Returns any data previously set on the node via setUserData() by key
* [[Node.hasAttributes]]: Indicates whether the node possesses attributes
* [[Node.hasChildNodes]]: Returns a Boolean value indicating whether the current element has child nodes or not.
* [[document.hasFocus]]: Returns true if the focus is currently located anywhere inside the specified document.  
* [[document.importNode]]: Returns a clone of a node from an external document
* [[Node.insertBefore]]: Inserts the specified node before a reference node as a child of the current node.
* [[Node.isDefaultNamespace]]: Returns true if the namespace is the default namespace on the given node
* [[Node.isEqualNode]]: Indicates whether the node is equal to the given node
* [[Node.isSameNode]]: Indicates whether the node is the same as the given node
* [[Node.isSupported]]: Tests whether the DOM implementation implements a specific feature and that feature is supported by this node or document
* [[document.load]]: Load an XML document
* [[Node.lookupNamespaceURI]]: Returns the namespaceURI associated with a given prefix on the given node object  
* [[Node.lookupPrefix]]: Returns the prefix for a given namespaceURI on the given node if present
* [[Node.normalize]]: Normalizes the node or document
* [[document.normalizeDocument]]: Replaces entities, normalizes text nodes, etc.
* [[document.open*]]: Opens a document stream for writing.
* [[document.queryCommandEnabled*]]: Returns true if the Midas command can be executed on the current range.
* [[document.queryCommandIndeterm*]]: Returns true if the Midas command is in a indeterminate state on the current range.
* [[document.queryCommandState*]]: Returns true if the Midas command has been executed on the current range.
* [[document.queryCommandSupported]]
* [[document.queryCommandText]]: document.queryCommandValue*]]: Returns the current value of the current range for Midas command. As of Firefox 2.0.0.2, queryCommandValue will return an empty string when a command value has not been explicitly set.
* [[document.querySelector]]: Returns the first Element node within the document, in document order, that matches the specified selectors.
* [[document.querySelectorAll]]: Returns a list of all the Element nodes within the document that match the specified selectors.
* [[document.releaseCapture]]: Releases the current mouse capture if it's on an element in this document.
* [[document.releaseEvents]]
* [[Node.removeChild]]: Removes a child node from the DOM
* [[document.removeEventListener]]: Removes an event listener from the document
* [[Node.replaceChild]]: Replaces one child node of the specified node with another
* [[document.routeEvent]]:
* [[document.mozSetImageElement]]: Allows you to change the element being used as the background image for a specified element ID.
* [[Node.setUserData]]: Attaches arbitrary data to a node, along with a user-defined key and an optional handler to be triggered upon events such as cloning of the node upon which the data was attached
* [[document.write*]]: Writes text to a document.
* [[document.writeln* ]]: Write a line of text to a document.

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
* [[addEventListener( type, listener, useCapture )]]: Bind an event callback to a specific event type on the element.
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
