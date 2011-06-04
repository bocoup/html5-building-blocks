The load method helps you programmatically control either the `[[audio]]` and `[[video]]` elements using JavaScript. 
This method is used to load a new source into the src attribute of the media tag. This method must be called after the src of an audio or video element is changed.

    document
      .querySelector('audioOrVideoSelector')
      .load()