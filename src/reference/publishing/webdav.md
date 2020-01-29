# WebDAV

Web Distributed Authoring and Versioning (WebDAV) is an extension of the Hypertext Transfer Protocol (HTTP) that allows client to perform remote Web content authoring operations. 

For publishing and subscribing via FTP you first need a WebDAV server. You can either use an existing WebDAV server from the internet (many easily available) or you can install your own. Before doing that you should first check whether other existing publication targets are available.

* File/folder in the local network
* FTP
* Cloud Storage Service (DropBox, Microsoft OneDrive, Google Drive)

If for some reason none of the above are possible then you can get started with your own WebDAV server. Windows Server provide a built-in WebDAV Server service. You simply need to activate this function. If for example you would like to install an WebDAV server under Windows 2012 just google "set up WebDAV windows server 2012" for equivalent instructions.

You can also set up an WebDAV Server on Linux. 

Once the WebDAV server is ready you can publish and subscribe to it. In both cases you will need to configure in SHOWTIME where your WebDAV is located and how to access it.

To connect to an WebDAV server from SHOWTIME DESIGNER proceed as follows:

1. Click on  `Project > Manage Publication Targets > FTP and WebDAV Server`.

2. Click on  `Add`.

3. Enter a name for the new publication target and select the entry "Folder on an WebDAV server".

4. Under `Hostname` enter the URL in which the desired folder exists.
   
   Examples:
   
   ```
http://www.myserver.de
http://www.myserver.de/shared
http://192.168.0.21
http://192.168.0.21/shared
   ```

5. The port specification `Port 80 or 443` is the standard port for the 80 or 443 protocol. Generally there's no need to change this. 

6. If access is protected uncheck the option `Login anonymously` and enter your username and password.

7. Click on `Test WebDAV Server` to test the connection to the WebDAV server.

8. If the connection test was successful click on `OK`.


