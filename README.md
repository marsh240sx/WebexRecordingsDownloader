Simple application to collect all Webex recordingIds and associated hostEmails and then download all recordings locally. 

It is a two step process which requires the app to be ran twice. 

On first run choose option 1 and provide your Webex site URL. For example, *sitename.webex.com*. 
* This collects all recordingIds and hostEmails and stores them in the recordings.csv file.
* The app will terminate itself after completion. 

Run the app again choose option 2.
* This will download all recordings that were retrived from step 1 and save them to the "Downloaded-Recordings" folder.

Setup:
* Create an [Integration](https://developer.webex.com/docs/integrations) or [Service App](https://developer.webex.com/docs/service-apps) with the admin and compliance related recording scopes.
* Generate your access and refresh tokens
* Add your Client ID, Client Secret and Refresh Token to the [.env](.env) file. 
* You can also add your Access Token to the [token.json](token.json) file but the app will handle adding that for you when you run option 1 if you don't.

Start the app from terminal/command line:
* ``python recordings.py``
  
