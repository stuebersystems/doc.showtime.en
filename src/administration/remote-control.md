# Remote Control

Even when everything's working well and perfectly automated you may still wish to take a look at the computer of your public display from time to time to install system updates, install new software etc. 

The simplest way to do is to connect to the computer via remote control software. Windows provides a built-in tool *Remote Desktop Connection*. Do the following in order to use it:

1. Set up the computer of the public display to allow it to use Remote Desktop connections.

  1. Open the control panel and click on `System`.

  2. Now click on `Remote settings`. A dialog window open. If an Administrator permission is required, you may be prompted for an administrator password or to confirm the selection.

  3. Select one of the two options `Allow connections...` and confirm by clicking `OK`.

  4. In order to ensure the computer is always online and available we highly recommend the computer uses the "High performance" power plan and the setting "Never: Put the computer to sleep" under Power Options. 

2. On your workstation start the application `Remote Desktop Connection` and enter the name or IP address of the public display.

3. Click `Connect` to start a connection to the Public Display computer. If you prompted for a user name and password enter both in.

Within your local network you there is not much to worry about, however from home or working remotely it is recommended to use a VPN (Virtual Private Network) connection to access your public display. This allows a secure communication between yourself and your public display over the internet.

There are of course alternatives to *Remote Desktop Connection* such as [TeamViewer](http://www.teamviewer.com) or the Open Source solution [VNC](http://www.tightvnc.com).
