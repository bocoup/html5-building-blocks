The `playbackRate` property is available to you on the `[[audio]]` or `[[video]]` elements via JavaScript.

###[[volume|media-volume-property]]
This property contains the volume (0 - 9) of the selected media element. This property is only available after the video is loaded with the load method.

    document
      .querySelector('audioOrVideoSelector')
      .volume // returns the current playback rate

      document
        .querySelector('audioOrVideoSelector')
        .volume = 8 // make it almost as loud as it can go

###[[duration|media-duration-property]]
This property contains the total duration in milliseconds of the selected media element. This property is only available after the video is loaded with the load method.

    document
      .querySelector('audioOrVideoSelector')
      .duration // returns the current playback rate
