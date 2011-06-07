Session storage is a key value store that allows you to persist serialized objects in [[JSON]] format for a single user session. Session storage persists until the user closes the browser window running your program. Session storage is similar to [[Local Storage]] which behaves the same way, but persists until the user clears their browsing data in the browser settings.

##Usage:
    var myJSONString = JSON.stringify({
      propery: 'myfavevalue',
      anotherProp: ['my', 'fave', 'array', 'of', 'strings']
    });

    window.localStorage.setItem( 'myData', myJSONString );

    window.localStorage.getItem( 'myData' ) //returns myJSONString
