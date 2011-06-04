The load method helps you programmatically control either the `[[audio]]` and `[[video]]` elements using JavaScript. 
This method causes the selection to stop playing if it is playing, and does nothing if it is not playing.

    document
      .querySelector('audioOrVideoSelector')
      .pause()