This is a helper App for learning the LookbackAPI that was created for the 2012 RallyOn Hackathon. It requires the Lookback API to function.



Since this app was created as part of the hackathon it is not guaranteed to work.
    

To launch chrome with cross-origin checks and file access checks disabled, on windows it will look something like:

    %LOCALAPPDATA%\Google\Chrome\Application\chrome.exe --disable-web-security --allow-file-access-from-files --allow-cross-origin-auth-prompt

On mac:

    cd /Applications
    open Google\ Chrome.app --args --disable-web-security --allow-file-access-from-files --allow-cross-origin-auth-prompt

The first time you run the app you'll be prompted with a browser auth window from rally1.rallydev.com for the 'Rally ALM' security realm.
Also, the first time you search you'll get another auth prompt, this time for the 'Rally Analytics API' realm.
You should only need to do these once and then the browser will cache it for the rest of your session (until the browser is closed).
This is only a temporary limitation, which will be resolved in the final version of the analytics API, when we have integrated authentication with Rally ALM.

Live JSFiddle Example:
http://jsfiddle.net/markmsmith/MBSpX/