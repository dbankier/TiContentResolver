# TiContent for Android

Resolves content uri to their native path.
_Very_ useful when using intents to, e.g. record audio.



## Usage


~~~
// if returned something like this from an intent:
var contentUri = "content://media/external/audio/media/635";

var Content = require("yy.ticontent");
var nativePath = Content.resolveAudioPath(contentUri);
alert("Native Path: file://" + nativePath);
~~~

Supports the following commands:

~~~
Content.resolveAudioPath(contentUri);
Content.resolveImagePath(contentUri);
Content.resolveVideoPath(contentUri);
~~~


###Licence: MIT
