Local storage is a key value store that allows you to persist serialized objects in [[JSON]] format across user sessions. Local storage persists until the user clears their browsing data in the browser settings. Local storage is similar to [[Session Storage]] which behaves the same way, but deletes stored objects when a browsing session is closed.

##Usage:
    var myJSONString = JSON.stringify({
      propery: 'myfavevalue',
      anotherProp: ['my', 'fave', 'array', 'of', 'strings']
    });

    window.localStorage.setItem( 'myData', myJSONString );

    window.localStorage.getItem( 'myData' ) //returns myJSONString
