The load method helps you programmatically control either the `[[audio]]` and `[[video]]` elements using JavaScript. 
This method causes the selection to start playing if it is not playing, and does nothing if it is already playing.

    document
      .querySelector('audioOrVideoSelector')
      .play()