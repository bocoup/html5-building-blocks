This is the documentation for the JavaScript interface to the [[audio-tag|html audio element]]

<a href="http://www.w3.org/2010/05/video/mediaevents.html">W3C Media Events Demo Page</a>


##Every Media Event:
Bind to these events with

    document
      .querySelector('audioselector')
      .addEventListener('eventname', function( eventObj ){
        // do stuff in response to the event
        // log eventObj, it has interesting stuff
      })
      

###abort
Sent when playback is aborted; for example, if the media is playing and is restarted from the beginning, this event is sent.

###canplay
Sent when enough data is available that the media can be played, at least for a couple of frames.  This corresponds to the CAN_PLAY readyState.

###canplaythrough
Sent when the ready state changes to CAN_PLAY_THROUGH, indicating that the entire media can be played without interruption, assuming the download rate remains at least at the current level.

###canshowcurrentframe
The current frame has loaded and can be presented.  This corresponds to the CAN_SHOW_CURRENT_FRAME readyState.

###dataunavailable
Sent when the ready state changes to DATA_UNAVAILABLE.

###durationchange
The metadata has loaded or changed, indicating a change in duration of the media.  This is sent, for example, when the media has loaded enough that the duration is known.

###emptied
The media has become empty; for example, this event is sent if the media has already been loaded (or partially loaded), and the load() method is called to reload it.

###empty
Sent when an error occurs and the media is empty.

###ended
Sent when playback completes.

###error
Sent when an error occurs.  The element's error attribute contains more information. See Error handling for details.

###loadeddata
The first frame of the media has finished loading.

###loadedmetadata
The media's metadata has finished loading; all attributes now contain as much useful information as they're going to.

###loadstart
Sent when loading of the media begins.

###pause
Sent when playback is paused.

###play
Sent when playback of the media starts after having been paused; that is, when playback is resumed after a prior pause event.

###playing
Sent when the media begins to play (either for the first time, after having been paused, or after ending and then restarting).

###progress
Sent periodically to inform interested parties of progress downloading the media. Information about the current amount of the media that has been downloaded is available in the media element's buffered attribute.

###ratechange
Sent when the playback speed changes.

###seeked
Sent when a seek operation completes.

###seeking
Sent when a seek operation begins.

###timeupdate
The time indicated by the element's currentTime attribute has changed.

###volumechange
Sent when the audio volume changes (both when the volume is set and when the muted attribute is changed).

###waiting
Sent when the requested operation (such as playback) is delayed pending the completion of another operation (such as a seek).
