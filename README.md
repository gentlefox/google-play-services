Repo contains the Google Play Services v24 / 7.3.27 library distributed
through the Android SDK Manager.

[1] https://developer.android.com/google/play-services

How to update to latest Google Play Services:
1. Replace the  libs/google-play-services_lib directory with the latest downloaded Google Play Service by the Android SDK from your local downloaded directory.
2. Find version number of latest downloaded Google Play Service directory under:
    google-play-services_lib>res>values>version.xml
3. Copy this number to version.xml of this plugin.
4. Update the version number in plugin.xml of this plugin.


THIS PLUGIN SHOULD BE DEPRECATED!!!
Plugins should use framework tags instead.
E.g.:
    &lt;framework src="com.google.android.gms:play-services-plus:+" /&gt;
    &lt;framework src="com.google.android.gms:play-services-identity:+" />&gt;
Full list available: http://developer.android.com/google/play-services/setup.html

But this does currently not work under phonegap build 3.7.0. so use this instead:
	<dependency id="com.google.playservices" url="https://github.com/LogicsSoftware/google-play-services.git" />
