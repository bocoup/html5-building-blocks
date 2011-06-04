The `playbackRate` property is available to you on the `[[audio]]` or `[[video]]` elements via JavaScript.

This property contains the playback rate of the selected media element. You can access it at any time during playback, or when it is paused. Changing the value of this property to a different number, will cause the media to play that many times faster or slower the next time the media is playing. If the media is already playing, then changing this property will take immediate effect on the next time update. This property is only available after the video is loaded with the load method.

    document
      .querySelector('audioOrVideoSelector')
      .playbackRate // returns the current playback rate

      document
        .querySelector('audioOrVideoSelector')
        .playbackRate = 15 // make the media play 15 times faster than normal

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
