These methods are available for you to programmatically control either the `[[audio]]` or `[[video]]` elements using JavaScript.

###[[load|media-load-method]]
This method is used to load a new source into the src attribute of the media tag. This method must be called after the src of an audio or video element is changed.

    document
      .querySelector('audioOrVideoSelector')
      .load()


###[[play|media-play-method]]
This method causes the selection to start playing if it is not playing, and does nothing if it is already playing.

    document
      .querySelector('audioOrVideoSelector')
      .play()

###[[pause|media-pause-method]]
This method causes the selection to stop playing if it is playing, and does nothing if it is not playing.

    document
      .querySelector('audioOrVideoSelector')
      .pause()

###[[mute|media-lomutead-method]]
This method causes the selection's volume property to be set to 0.

    document
      .querySelector('audioOrVideoSelector')
      .mute()