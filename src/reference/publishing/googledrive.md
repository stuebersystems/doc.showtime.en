# Google Drive


Google Drive is a file hosting service for sharing and managing files. You can register for free at https://www.google.com/intl/en/drive and start uploading files straight away.

Once you have a Google Drive account you can use it to publish and subscribe using CONFIRE SHOWTIME. There are just some simple steps you first need to follow in order to grant both SHOWTIME DESIGNER and SHOWTIME PLAYER access to use it.


Proceed as follows:

1. Click on  `Project > Manage Publication Targets > Cloud Storage Service`.

2. Click on `Add`.

3. Enter a name for your new Publication Target and under `Provider` select the option `Google Drive`.

4. Click on `Authorise` to log into a Google Drive account with CONFIRE SHOWTIME. A dialog window opens.

5. Now log into Google Drive an by entering your email and password and then clicking `Sign in` to confirm. If the login is successful you then to select the button allow CONFIRE SHOWTIME access to your Google Drive account.

6. Google Drive will now generate an access key (access token) allowing you to access Google Drive securely without needing to manually log in again.

7. Then click on `OK`. 
   
The whole process of authorizing with Google Drive takes place using OAuth2 standards. When a user successfully logs in, Google Drive generates an access token and sends it back to CONFIRE SHOWTIME. An access token is a time limited key used for authorizing with Google Drive again at a later stage. If you want to generate a new access token click on `Authorize` in the dialog window once again.
