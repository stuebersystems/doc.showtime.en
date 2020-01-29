# Publish to DropBox

To publish projects in CONFIRE SHOWTIME DESIGNER to DropBox you need to first define the access settings to DropBox:

1. Click on  `Project > Manage Publication Targets > Cloud Storage Service`. A dialog window opens.

2. Click on `Add`.

3. Enter a name for your new Publication Target and under `Provider` select the option `DropBox`.

4. Click on `Autorisieren` to log into a Dropbox account with CONFIRE SHOWTIME. A dialog window opens.
   
   ![Anmeldung an DropBox](../../images/sign-in-dropbox.png)

5. Now log into DropBox an by entering your email and password and then clicking `Sign in` to confirm. If the login is successful you then to select the button allow CONFIRE SHOWTIME access to your DropBox account.

6. DropBox will now generate an access key (Access-Token) allowing you to access DropBox securely without needing to manually log in again.
   
   ![Dialog zum Hinzufügen eines DropBox-Speichers](../../images/add-dropbox.png)

6. Click on `OK`.  DropBox will now appear in the list of Cloud Storage Services.

7. Click on `Close`.

Now you can publish:

1. Open the desired project.

2. Click on `Project > Publish`. A wizard will open.

3. Select the publication target `Cloud Storage Service` and click `Continue`.
   
   ![Publizieren nach DropBox](../../images/publish-dropbox.png)
   
4. Now select the previously defined DropBox Storage and click on `Publish`. If you wish to change the name of the subfolder of the resulting project archive, click on the `...` button next to `Project archive`.

5. When you're happy with your selections click `Publish`. 

CONFIRE SHOWTIME creates a project archive and copies it to DropBox. As soon as you make any further changes to your project, publish it once again. CONFIRE SHOWTIME remembers the last place you saved to so that you can repeat this process with just a few clicks.

See more information on DropBox publication targets in the following [Reference Chapter](../../reference/publishing/dropbox.md).