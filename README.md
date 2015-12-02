# Play Services for Cordova

This is a simple Cordova plugin that adds the [Google Play Services](http://developer.android.com/google/play-services/setup.html)
client library to your app.

## Developer Guide

Repo contains the Google Play Services v28 / 8.3.0 library distributed
through the Android SDK Manager.<br>

[1] https://developer.android.com/google/play-services<br>

### How to update to latest Google Play Services

1. Replace the libs/google-play-services_lib directory with the latest downloaded Google Play Service by the Android SDK from your local downloaded directory.
  Normally under `[Android SDK] > extras > google > google_play_services > libproject`
2. Find version number of latest downloaded Google Play Service directory under:
  `google-play-services_lib > res > values > version.xml`
3. Copy this number to version.xml of this plugin.
4. Update the version number in plugin.xml of this plugin.

THIS PLUGIN SHOULD BE DEPRECATED!!!<br>

Plugins should use framework tags instead.<br>
E.g.:<br>
    &lt;framework src="com.google.android.gms:play-services-plus:+" /&gt;<br>
    &lt;framework src="com.google.android.gms:play-services-identity:+" />&gt;<br>
Full list available: http://developer.android.com/google/play-services/setup.html<br>

But unfortunately some systems are "safe" to the point of waiting until components are near legacy or deprecated before updating.

This includes:

* PhoneGap up to build 3.7.0
* FeedHenry version 3.3 (although support appears to be coming for the upcoming 3.6 release!)

If stuck in the past using clunky manual compilation of outdated plugins and dependencies, or simply wish to avoid using Gradle, use this instead:

< dependency id="com.google.playservices" url="https://github.com/gentlefox/google-play-services.git" />
