# UnityPlugin
It is a plugin for Unity to add the indiexpo Score System to your WebGL games.

With this plugin you'll be able to send user's score to the Indiexpo's server, it work only for WebGl builds.

To install this plugin simply import IndiexpoAPI_WebGL.unitypackage in Unity or run IndiexpoAPI_WebGL.unitypackage and follow the instructions;

After the installation make sure that the file IndiexpoAPI_Plugin.jslib is correctly placed in:
your_project_folder\Assets\Plugins

To send score you only need to use this code: 
IndiexpoAPI_WebGL.SendScore(100); 
where 100 is the score.

## EXTRA
You can also, if you want, show a message box in the user's browser, to do so use this code:
IndiexpoAPI_WebGL.SendMessage(TEXT);
where TEXT is the message that you want to show.

Thanks to Marty for the help!

P.S. the Score System is a Beta feature, now only for few Devs. If you want to be in the List, contact the staff from the website.

indiexpo Staff
