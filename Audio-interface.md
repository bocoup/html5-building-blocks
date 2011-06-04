This is the documentation for the JavaScript interface to the [[html audio element|audio]]. The audio tag JavaScript interface is very similar to the [[video interface]]. Both interfaces are constructed from the HTMLMediaElement.


##Every Audio Method:
Use these methods by

    document
      .querySelector('audioselector')
      .methodName()

###load
This method is used to load a new source into the src attribute of the audio tag. This method must be called after the src of an audio element is changed.

    document
      .querySelector('audioselector')
      .load()


###play

###pause

###mute

##Every Audio Property:

###currentTime

###playbackRate

###volume

###duration

###networkState

##Every Audio Event:
The `audio` element event interface has a lot in common with the `[[video interface]]`. Both interfaces are based of the [[media events]] interface.

You can Bind to these events with

    document
      .querySelector('audioselector')
      .addEventListener('eventname', function( eventObj ){
        // do stuff in response to the event
        // log eventObj, it has interesting stuff
      })
      
A useful demo of all of the events bellow is available on the <a href="http://www.w3.org/2010/05/video/mediaevents.html">W3C Media Events Demo Page</a> (note that this demo page uses a video to demonstrate the event interfaces).

The following events are available to you when adding event listeners (or 'binding') to the audio element:

`[[abort]], [[canplay]], [[canplaythrough]], [[canshowcurrentframe]], [[dataunavailable]], [[durationchange]], [[emptied]], [[empty]], [[ended]], [[error]], [[loadeddata]], [[loadedmetadata]], [[loadstart]], [[pause]], [[play]], [[playing]], [[progress]], [[ratechange]], [[seeked]], [[seeking]], [[timeupdate]], [[volumechange]], [[waiting]]`