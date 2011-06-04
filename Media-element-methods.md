###[[load|media-load-method]]
This method is used to load a new source into the src attribute of the audio tag. This method must be called after the src of an audio element is changed.

    document
      .querySelector('audioselector')
      .load()


###[[play|media-play-method]]
This method causes the selection to start playing if it is not playing, and does nothing if it is already playing.

    document
      .querySelector('audioselector')
      .play()

###[[pause|media-pause-method]]
This method causes the selection to stop playing if it is playing, and does nothing if it is not playing.

    document
      .querySelector('audioselector')
      .pause()

###[[mute|media-lomutead-method]]
This method causes the selection's volume property to be set to 0.

    document
      .querySelector('audioselector')
      .mute()