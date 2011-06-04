##How it works:
    <tag attribute="value">
        contents
    </tag>

##Every HTML Tag:

[[a]], [[abbr]], [[acronym]], [[address]], [[area]], [[b]], [[base]], [[bdo]], [[big]], [[blockquote]], [[body]], [[br]], [[button]], [[caption]], [[cite]], [[dcode]], [[col]], [[colgroup]], [[dd]], [[del]], [[dfn]], [[div]], [[dl]], [[DOCTYPE]], [[dt]], [[em]], [[fieldset]], [[form]], [[h1, h2, h3, h4, h5, and h6]], [[head]], [[html]], [[hr]], [[i]], [[img]], [[input]], [[ins]], [[kbd]], [[label]], [[legend]], [[li]], [[link]], [[map]], [[meta]], [[noscript]], [[object]], [[ol]], [[optgroup]], [[option]], [[p]], [[param]], [[pre]], [[q]], [[samp]], [[script]], [[select]], [[small]], [[span]], [[strong]], [[style]], [[sub]], [[sup]], [[table]], [[tbody]], [[td]], [[textarea]], [[tfoot]], [[th]], [[thead]], [[title]], [[tr]], [[tt]], [[ul]], [[var]], [[article]], [[aside]], [[audio]], [[canvas]], [[datalist]], [[details]], [[figcaption]], [[figure]], [[footer]], [[header]], [[hgroup]], [[mark]], [[meter]], [[nav]], [[output]], [[progress]], [[section]], [[summary]], [[time]], [[video]]

##Every HTML Attribute
Every HTML element supports the following attributes (Note, many elements have additional support for element specific attributes): `id, class, style, tabindex, title, accesskey, contenteditable, dir, draggable, hidden, data-*, lang`. Each attribute is described below.

###id
This attribute defines a unique identifier (ID) which must be unique in the whole document. Its purpose is to identify the element when linking (using a fragment identifier), scripting, or styling (with CSS).

    Usage note:
    This attribute's value is an opaque string: this means that web author must not use it to convey any information. Particular meaning, for example semantic meaning, must not be derived from the string.
    This attribute's value must not contain white spaces. Browsers treat non-conforming IDs that contains white spaces as if the white space is part of the ID.  In contrast to the class attribute, which allows space-separated values, elements can only have one single ID defined through the id attribute. Note that an element may have several IDs, but the others should be set by another means, such as via a script interfacing with the DOM interface of the element. 
    Using characters except ASCII letters and digits, '_', '-' and '.' may cause compatibility problems, as they weren't allowed in HTML 4. Though this restriction has been lifted in HTML 5, an ID should start with a letter for compatibility purpose.

###class
This attribute is a space-separated list of the classes of the element. Classes allows CSS and Javascript to select and access specific elements via the class selectors or functions like the DOM method document.getElementsByClassName().
Usage note: Though the specification doesn't put requirements on the name of classes, web developers are encouraged to use names that describe the semantic purpose of the element, rather to the presentation of the element (e.g., attribute to describe an attribute rather than italics, although an element of this class may be presented by italics). Semantic names remain logical even if the presentation of the page changes.

###style
This attribute contains CSS styling declarations to be applied to the element. Note that it is recommended for styles to be defined in a separate file or files. This attribute and the &lt;style&gt; element have mainly the purpose of allowing for quick styling, for example for testing purposes.
Usage note: This attribute must not be used to convey semantic information. Even if all styling is removed, a page should remain semantically correct. Typically it shouldn't be used to hide irrelevant information; this should be done using the hidden attribute.

###tabindex
This integer attribute indicates if the element can take input focus (is focusable), if it should participate to sequential keyboard navigation, and if so, at what position. It can takes several values:

* a negative value means that the element should be focusable, but should not be reachable via sequential keyboard navigation;
* 0 means that the element should be focusable and reachable via sequential keyboard navigation, but its relative order is defined by the platform convention;
* a positive value which means should be focusable and reachable via sequential keyboard navigation; its relative order is defined by the value of the attribute: the sequential follow the increasing number of the tabindex. If several elements share the same tabindex, their relative order follows their relative position in the document).

An element with a 0 value, an invalid value, or no tabindex value should be placed after elements with a positive tabindex in the sequential keyboard navigation order.


###title
This attribute contains a text representing advisory information related to the element it belongs too. Such information can typically, but not necessarily, be presented to the user as a tooltip. Here are some typical uses of this attribute:

* Link: the title or a description of the linked document
* Media element like an image: a description or associated credits
* Paragraph: a footnote or a commentary about it
* Quotation: some information about the author, and so on.

If this attribute is omitted, it means that the title of the nearest ancestor of this element is still relevant for it (and can legitimately be used as the tooltip for that element. If this attribute is set to the empty string, it explicitly means that its nearest ancestor's title is not relevant for this element (and shouldn't be used in the tooltip for that element).

Additional semantics are attached to the title attributes of the &lt;link&gt;, &lt;abbr&gt; and &lt;input&gt;.

    Usage note:
    The title attribute may contains several lines. Each U+000A LINE FEED (LF) inserted represents such a newline. Some caution must be taken though, as that means that:

###accesskey
This attribute provides a hint for generating a keyboard shortcut for the current element. This attribute consists of a space-separated list of characters (one single Unicode code point). The browser should use the first one that exists on the computer keyboard layout.


###contenteditable
This enumerated attribute indicates if the element should be editable by the user. If so, the browser modifies its widget to allow editing. The attribute must take one of the following values:
true or the empty string, which indicates that the element must be editable;
false, which indicates that the element must not be editable.
If this attribute is not set, its default value is inherited from its parent element.

    Usage note: This attribute is an enumerated one and not a Boolean one. This means that the explicit usage of one of the values true, false or the empty string is mandatory and that a shorthand like <label contenteditable>Example Label</label> is not allowed. The correct usage is <label contenteditable="true">Example Label</label>.

###dir
This enumerated attribute indicates the directionality of the element's text. It can have the following values:
ltr, which means left to right and is to be used for languages that are written from the left to the right (like English);
rtl, which means right to left and is to be used for languages that are written from the right to the left (like Arabic).

    Usage notes:
    This attribute can be overrided by the CSS properties direction and unicode-bidi , if a CSS page is active and the element supports these properties.
    As the directionality of the text is semantically related to its content and not to its presentation, it is recommended that web developers use this attribute instead of the related CSS properties when possible. That way, the text will display correctly even on a browser that doesn't support CSS or has the CSS deactivated.
    This attribute is mandatory for the <bdo> element. 


###draggable
This enumerated attribute indicates whether the element can be dragged, using the Drag and Drop API. It can have the following values:
true, which indicates that the element may be dragged
false, which indicates that the element may not be dragged.
If this attribute is not set, its default value is auto, meaning the behavior should be the one defined by default by the browser.

    Usage notes:
    This attribute is an enumerated one and not a Boolean one. This means that the explicit usage of one of the values true or false is mandatory and that a shorthand like <label draggable>Example Label</label> is not allowed. The correct usage is <label draggable="true">Example Label</label>.
    By default, only text selections, images, and links can be dragged. For all others elements, the event ondragstart must be set in order to the drag and drop mechanism to work, as shown in this comprehensive example.


###hidden
This Boolean attribute indicates that the element is not yet, or is no longer, relevant. For example, it can be used to hide elements of the page that can't be used until the login process has been completed. The browser won't render such elements.

    Usage notes:
    This attribute must not be used to hide content that could be legitimately be shown. For example, it shouldn't be used to hide tabs panels of a tabbed interface, as this is a styling decision and another style showing them would lead to a perfectly correct page.
    Hidden elements shouldn't be linked from non-hidden elements.
    Elements that are descendants of a hidden element are still active, which means that script elements can still execute and form elements can still submit.

###data-*
This class of attributes, called custom data attributes, allows proprietary information to be exchanged between the HTML and its DOM representation that may be used by scripts. All such custom data are available via the HTMLElement interface of the element the attribute is set on. The HTMLElement.dataset property gives access to them.
The * may be replaced by any name following the production rule of xml names with the following restrictions:

    * the name must not start with xml, whatever case is used for these letters;
    * the name must not contain any semicolon (U+003A);
    * the name must not contain capital A to Z letters.

Note that the HTMLElement.dataset attribute is a StringMap and the name of the custom data attribute data-test-value will be accessible via HTMLElement.dataset.testValue as any dash (U+002D) is replaced by the capitalization of the next letter (camelcase).

###lang
This attribute participates in defining the language of the element, the language that non-editable elements are written in or the language that editable elements should be written in. The tag contains one single entry value in the format defines in the Tags for Identifying Languages (BCP47) IETF document. If the tag content is the empty string the language is set to unknown; if the tag content is not valid, regarding to BCP47, it is set to invalid.

    Usage note: 
    Even if the lang attribute is set, it may not be taken into account, as the xml:lang attribute has priority. Read the algorithm determining the language of an element's content to see how the language is determined in all cases.
    For the CSS pseudo-class :lang , two invalid language names are different if their names are different.