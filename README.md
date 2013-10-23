HypMedias
=========

Haxe NME / OpenFL extension for Media Playback

Vidéo playback only for now, and soon recording, display image...

__Install:__

On haxelib ( haxe 3 ):
```java
haxelib install HypMedias
```

Or clone the repository.

You need to install ( and link it in your project.xml ) the haxelib "inthebox-macros"
```java
haxelib install inthebox-macros
```

HypVideo:
-----------------------------

Allow to play Videos on Android & iOS

__Usage:__

The usage is quite simple:
```java
var v = HypVideo.getInstance( );
	v.addEventListener( HypVideoEvent.PLAYBACK_COMPLETE , _onHypVideo_event );
	v.addEventListener( HypVideoEvent.PLAYBACK_ERROR , _onHypVideo_event );
	v.addEventListener( HypVideoEvent.PLAYBACK_INFO , _onHypVideo_event );
	v.addEventListener( HypVideoEvent.PLAYBACK_PAUSE , _onHypVideo_event );
	v.addEventListener( HypVideoEvent.PLAYBACK_PLAY , _onHypVideo_event );
	v.addEventListener( HypVideoEvent.PLAYBACK_SEEK , _onHypVideo_event );
	v.addEventListener( HypVideoEvent.PLAYBACK_STOP , _onHypVideo_event );
	v.playRemote("VIDEOURL");
```

Take a look at the "demo" folder for a ready to compile demo.

__iOS setup:__

Nothing to do.

__Android setup:__

For android you need to add the following activity to your AndroidManifest:
```xml
<!-- HypMedias -->
<activity
	android:name="fr.hyperfiction.hypmedias.HypVideoActivity"
	android:theme="@android:style/Theme.NoTitleBar.Fullscreen"
	android:label="HypMedias"
	android:screenOrientation="landscape"
/>
```

Made at [Hyperfiction](http://hyperfiction.fr)
--------------------
Developed by [Johann Martinache](https://github.com/shoebox) [@shoe_box](https://twitter.com/shoe_box)

License
-------
This work is under BSD simplified License.
