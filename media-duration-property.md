The `playbackRate` property is available to you on the `[[audio]]` or `[[video]]` elements via JavaScript.

###[[duration|media-duration-property]]
This property contains the total duration in milliseconds of the selected media element. This property is only available after the video is loaded with the load method.

    document
      .querySelector('audioOrVideoSelector')
      .duration // returns the current playback rate
