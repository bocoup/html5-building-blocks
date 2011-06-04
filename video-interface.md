This is the documentation for the JavaScript interface to the [[html video element|video]]. The video element JavaScript interface is very similar to the [[audio interface]].


##video Methods:
[[load|media-load-method]], [[play|media-play-method]], [[pause|media-pause-method]], [[mute|media-lomutead-method]]

###How to use these methods
The `video` element has the same methods as the `audio` element.

    document
      .querySelector('videoselector')
      .methodName() // calls the method on the selection

For an overview of each method, see [[Media Element Methods]].

##video Properties:
The `video` element has the same properties as the `video` element.

`[[currentTime|media-currentTime-property]], [[playbackRate|media-playbackRate-property]], [[volume|media-volume-property]], [[duration|media-duration-property]], [[networkState|media-networkState-property]]`

###How to use these properties

    document
      .querySelector('videoselector')
      .propertyName // returns the value of the property

For an overview of each property, see [[Media Element Properties]].

##video Events:
The `video` element event interface is the same as the `[[audio interface]]`. Both interfaces are based on the [[media events]] interface.

The following events are available to you when adding event listeners (or 'binding') to the video element

`[[abort]], [[canplay]], [[canplaythrough]], [[canshowcurrentframe]], [[dataunavailable]], [[durationchange]], [[emptied]], [[empty]], [[ended]], [[error]], [[loadeddata]], [[loadedmetadata]], [[loadstart]], [[pause]], [[play]], [[playing]], [[progress]], [[ratechange]], [[seeked]], [[seeking]], [[timeupdate]], [[volumechange]], [[waiting]]`

A useful demo of all of the events bellow is available on the <a href="http://www.w3.org/2010/05/video/mediaevents.html">W3C Media Events Demo Page</a>.

###How to use these events

    // bind to an event
    document
      .querySelector('videoselector')
      .addEventListener('eventname', function( eventObj ){
        // do stuff in response to the event
        // log eventObj, it has interesting stuff
      })
      
