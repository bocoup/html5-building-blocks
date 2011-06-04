##Usage

    <video src="http://example.com/videofile.format">
        Text to show if video is not supported.
        Protip: you can put code in here to run if HTML video is unsupported
        like a flash fallback for example.
     </video>
In it's simplest form, the `video` tag takes an src attribute, and gives you the default browser styled video player. The optional attributes below give you more fined grained control over the default behavior of the video tag.

##Every video Attribute
In addition to supporting the default HTML element attributes which are `id, class, style, tabindex, title, accesskey, contenteditable, dir, draggable, hidden, data-*, lang`, the `video` tag also supports the following attributes:

###poster
A URL indicating a poster frame to show until the user plays or seeks. If this attribute isn't specified, nothing is displayed until the first frame is available; then the first frame is displayed as the poster frame.

###controls
If this attribute is present, Gecko will offer controls to allow the user to control video playback, including volume, seeking, and pause/resume playback.

###autoplay
A Boolean attribute; if specified, the video will automatically begin to play back as soon as it can do so without stopping to finish loading the data.

###height
The height of the video's display area, in CSS pixels.

###width
The width of the video's display area, in CSS pixels.

###autobuffer Obsolete in Gecko 2.0
A Boolean attribute; if specified, the video will automatically begin buffering even if it's not set to automatically play. This should be used for cases in which it is considered likely that the video will be played (for example, if the user navigated to the page specifically to play the video, not if there happens to be a video embedded along with other content). The video is buffered until the media cache is full.

###buffered
An attribute you can read to determine which time ranges of the media have been buffered. This attribute contains a TimeRanges object.

###loop
A Boolean attribute; if specified, we will, upon reaching the end of the video, automatically seek back to the start.

###preload Requires Gecko 2.0 bug 548523
This enumerated attribute is intended to provide a hint to the browser about what the author thinks will lead to the best user experience. It may have one of the following values:

* none: hints that either the author thinks that the user won't need to consult that video or that the server wants to minimize its traffic; in others terms this hint indicates that the video should not be cached;
* metadata: hints that though the author thinks that the user won't need to consult that video, fetching the metadata (e.g. length) is reasonable;
* auto: hints that the user needs have priority; in others terms this hint indicated that, if needed, the whole video could be downloaded, even if the user is not expected to use it;
* the empty string: which is a synonym of the auto value.

If not set, its default value is browser-defined (i.e. each browser can choose its own default value), though the spec advises it to be set to metadata.

    ####Usage notes:
    The autoplay attribute has precedence over this one as if one wants to automatically play a video, the browser will obviously need to download it. Setting both the autoplay and the preload attributes is allowed by the specification.
    The browser is not forced by the specification to follow the value of this attribute; it is a mere hint.

###src
The URL of the video to embed. This is optional; you may instead use the &lt;source&gt; element within the video block to specify the video to embed.
