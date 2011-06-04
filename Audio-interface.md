This is the documentation for the JavaScript interface to the [[html audio element|audio]]. The audio element JavaScript interface is very similar to the [[video interface]].


##Audio Methods:
[[load|media-load-method]], [[play|media-play-method]], [[pause|media-pause-method]], [[mute|media-lomutead-method]]

###How to use these methods
The `audio` element has the same methods as the `video` element.

    document
      .querySelector('audioselector')
      .methodName() // calls the method on the selection

For an overview of each method, see [[Media Element Methods]].

##Audio Properties:
The `audio` element has the same properties as the `video` element.

`[[currentTime|media-currentTime-property]], [[playbackRate|media-playbackRate-property]], [[volume|media-volume-property]], [[duration|media-duration-property]], [[networkState|media-networkState-property]]`

###How to use these properties

    document
      .querySelector('audioselector')
      .propertyName // returns the value of the property

For an overview of each property, see [[Media Element Properties]].

##Audio Events:
The `audio` element event interface is the same as the `[[video interface]]`. Both interfaces are based on the [[media events]] interface.

The following events are available to you when adding event listeners (or 'binding') to the audio element

`[[abort]], [[canplay]], [[canplaythrough]], [[canshowcurrentframe]], [[dataunavailable]], [[durationchange]], [[emptied]], [[empty]], [[ended]], [[error]], [[loadeddata]], [[loadedmetadata]], [[loadstart]], [[pause]], [[play]], [[playing]], [[progress]], [[ratechange]], [[seeked]], [[seeking]], [[timeupdate]], [[volumechange]], [[waiting]]`

A useful demo of all of the events bellow is available on the <a href="http://www.w3.org/2010/05/video/mediaevents.html">W3C Media Events Demo Page</a> (note that this demo page uses a video to demonstrate the event interfaces).

###How to use these events

    // bind to an event
    document
      .querySelector('audioselector')
      .addEventListener('eventname', function( eventObj ){
        // do stuff in response to the event
        // log eventObj, it has interesting stuff
      })
      
