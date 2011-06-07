Local storage is a key value store that allows you to persist serialized objects in [[JSON]] format across user sessions. Local storage persists until the user clears their browsing data in the browser settings. Local storage is similar to [[Session Storage]] which behaves the same way, but deletes stored objects when a browsing session is closed.

There is a great chapter on Local storage on [[diveintohtml5.org/storage.html|http://diveintohtml5.org/storage.html]]

##Usage:
    var myJSONString = JSON.stringify({
      propery: 'myfavevalue',
      anotherProp: ['my', 'fave', 'array', 'of', 'strings']
    });
    window.localStorage.setItem( 'myData', myJSONString );

    window.localStorage.getItem( 'myData' ) //returns myJSONString
