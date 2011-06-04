##Media Events
The following events are available to you when adding event listeners (or 'binding') to the `[[audio]]` or `[[video]]` elements.

###How to use these events

    // bind to an event
    document
      .querySelector('audioselector')
      .addEventListener('eventname', function( eventObj ){
        // do stuff in response to the event
        // log eventObj, it has interesting stuff
      })
      

A useful demo of all of the events bellow is available on the <a href="http://www.w3.org/2010/05/video/mediaevents.html">W3C Media Events Demo Page</a> (note that this demo page uses a video to demonstrate the events).

###List of media events:

####[[abort|media-abort-event]]
Fires when playback is aborted; for example, if the media is playing and is restarted from the beginning, this event is sent.

####[[canplay|media-canplay-event]]
Fires when enough data is available that the media can be played, at least for a couple of frames.  This corresponds to the CAN_PLAY readyState.

####[[canplaythrough|media-canplaythrough-event]]
Fires when the ready state changes to CAN_PLAY_THROUGH, indicating that the entire media can be played without interruption, assuming the download rate remains at least at the current level.

####[[canshowcurrentframe|media-canshowcurrentframe-event]]
The current frame has loaded and can be presented.  This corresponds to the CAN_SHOW_CURRENT_FRAME readyState.

####[[dataunavailable|media-dataunavailable-event]]
Fires when the ready state changes to DATA_UNAVAILABLE.

####[[durationchange|media-durationchange-event]]
The metadata has loaded or changed, indicating a change in duration of the media.  This is sent, for example, when the media has loaded enough that the duration is known.

####[[emptied|media-emptied-event]]
The media has become empty; for example, this event is sent if the media has already been loaded (or partially loaded), and the load() method is called to reload it.

####[[empty|media-empty-event]]
Fires when an error occurs and the media is empty.

####[[ended|media-ended-event]]
Fires when playback completes.

####[[error|media-error-event]]
Fires when an error occurs. The media element's error attribute contains more information. See Error handling for details.

####[[loadeddata|media-loadeddata-event]]
The first frame of the media has finished loading.

####[[loadedmetadata|media-loadedmetadata-event]]
The media's metadata has finished loading; all attributes now contain as much useful information as they're going to.

####[[loadstart|media-loadstart-event]]
Fires when loading of the media begins.

####[[pause|media-pause-event]]
Fires when playback is paused.

####[[play|media-play-event]]
Fires when playback of the media starts after having been paused; that is, when playback is resumed after a prior pause event.

####[[playing|media-playing-event]]
Fires when the media begins to play (either for the first time, after having been paused, or after ending and then restarting).

####[[progress|media-progress-event]]
Sent periodically to inform interested parties of progress downloading the media. Information about the current amount of the media that has been downloaded is available in the media element's buffered attribute.

####[[ratechange|media-ratechange-event]]
Fires when the playback speed changes.

####[[seeked|media-seeked-event]]
Fires when a seek operation completes.

####[[seeking|media-seeking-event]]
Fires when a seek operation begins.

####[[timeupdate|media-timeupdate-event]]
The time indicated by the media element's currentTime attribute has changed.

####[[volumechange|media-volumechange-event]]
Fires when the media element's volume changes (both when the volume is set and when the muted attribute is changed).

####[[waiting|media-waiting-event]]
Fires when the requested operation (such as playback) is delayed pending the completion of another operation (such as a seek).