###autoplay
A Boolean attribute; if specified (even if the value is "false"!), the audio will automatically begin to play back as soon as it can do so without stopping to finish loading the data.

###autobuffer Obsolete in Gecko 2.0
A Boolean attribute; if specified, the audio will automatically begin being downloaded, even if not set to automatically play. This continues until the media cache is full, or the entire audio file has been downloaded, whichever comes first. This should only be used when it is expected that the user will choose to play the audio; for example, if the user has navigated to a page using a "Play this audio" link. This attribute was removed in Gecko 2.0 (Firefox 4 / Thunderbird 3.3 / SeaMonkey 2.1) in favor of the preload attribute.

###buffered Requires Gecko 2.0
An attribute you can read to determine which time ranges of the media have been buffered. This attribute contains a TimeRanges object.

###controls
If this attribute is present, the browser will offer controls to allow the user to control audio playback, including volume, seeking, and pause/resume playback.

###loop Unimplemented bug 449157
A Boolean attribute; if specified, we will, upon reaching the end of the audio, automatically seek back to the start.

###mozCurrentSampleOffset Requires Gecko 2.0 Non-standard
The offset, specified as the number of samples since the beginning of the audio stream, at which the audio is currently playing.

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
The URL of the audio to embed. This is subject to HTTP access controls. This is optional; you may instead use the source element within the audio block to specify the audio to embed.