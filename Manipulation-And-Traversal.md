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
