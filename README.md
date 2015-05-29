Repo contains the Google Play Services v25 / 7.5.71 library distributed
through the Android SDK Manager.<br>

[1] https://developer.android.com/google/play-services<br>

How to update to latest Google Play Services:<br>
1. Replace the  libs/google-play-services_lib directory with the latest downloaded Google Play Service by the Android SDK from your local downloaded directory.<br>
normally under Android>extras>google>google_play_services>libproject<br>
2. Find version number of latest downloaded Google Play Service directory under:<br>
    google-play-services_lib>res>values>version.xml<br>
3. Copy this number to version.xml of this plugin.<br>
4. Update the version number in plugin.xml of this plugin.<br>


THIS PLUGIN SHOULD BE DEPRECATED!!!<br>
Plugins should use framework tags instead.<br>
E.g.:<br>
    &lt;framework src="com.google.android.gms:play-services-plus:+" /&gt;<br>
    &lt;framework src="com.google.android.gms:play-services-identity:+" />&gt;<br>
Full list available: http://developer.android.com/google/play-services/setup.html<br>

But this does currently not work under phonegap build 3.7.0. so use this instead:<br>
< dependency id="com.google.playservices" url="https://github.com/LogicsSoftware/google-play-services.git" commit="v25"/>
