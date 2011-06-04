The `currentTime` property is available to you on the `[[audio]]` or `[[video]]` elements via JavaScript.

This property contains the playback rate of the selected media element. You can access it at any time during playback, or when it is paused. Changing the value of this property to a different number, will cause the media to start the playhead at that number  the next time it is playing. If the media is already playing, then changing this property will cause it to skip to the new value set. This property is only available after the video is loaded with the load method.

    document
      .querySelector('audioOrVideoSelector')
      .currentTime // returns the current time

      document
        .querySelector('audioOrVideoSelector')
        .currentTime = 15 // move the playhead to 15 seconds