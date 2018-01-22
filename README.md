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
###### Check if the User is logged
You can check if who is playing your game is logged or not.
To make this you have to use function *IndiexpoAPI_WebGL.LoginCheck()*

*Example:*

        if (IndiexpoAPI_WebGL.LoginCheck() == true)
        {
            //add code that you want to run if the user is logged
        }
        else
        {
            //add code that you want to run if the user is not logged
        }

###### Show a Message Box
You can also, if you want, show a message box in the user's browser, to do so use this code:
IndiexpoAPI_WebGL.SendMessage(TEXT);
where TEXT is the message that you want to show.

###### Remember that...
...even if Unity's console in some case will show this error "EntryPointNotFoundException" your code is still fine, unfortunately the webGL's plugins needs to run in a browser otherwise they're not "seen" by Unity itself that will throw the aformentioned EntryPointNotFoundException error.
At this point there seem to be no solution to avoid this error other than building the game and then running locally in your webserver (you can use the build & run option in Unity) or by uploading the game to Indiexpo and then testing it.

Thanks to [Marty](https://www.indiexpo.net/users/emmetiennegames) for the help!

P.S. the Score System is a Beta feature, now only for few Devs. If you want to be in the List, contact the staff from the website.

*indiexpo Staff*
