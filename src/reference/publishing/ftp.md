# FTP

The File Transfer Protocol (FTP) is a very old but still popular network protocol for transferring files over IP networks. 

For publishing and subscribing via FTP you first need an FTP server. You can either use an existing FTP server from the internet (many easily available) or you can install your own. Before doing that you should first check whether other existing publication targets are available.

* File/folder in the local network
* WebDAV
* Cloud Storage Service (DropBox, Microsoft OneDrive, Google Drive)

If for some reason none of the above are possible then you can get started with your own FTP server. Windows Server provide a built-in FTP Server service. You simply need to activate this function. If for example you would like to install an FTP server under Windows 2012 just google "set up ftp windows server 2012" for equivalent instructions.

You can also set up an FTP Server on Linux. 

Once the FTP server is ready you can publish and subscribe to it. In both cases you will need to configure in SHOWTIME where your FTP is located and how to access it.

To connect to an FTP server from SHOWTIME DESIGNER proceed as follows:

1. Click on  `Project > Manage Publication Targets > FTP and WebDAV Server`.

2. Click on  `Add`.

3. Enter a name for the new publication target and select the entry "Folder on an FTP server".

4. Under `Hostname` enter the URL in which the desired folder exists.
   
   Examples:
   
   ```
   ftp://ftp.myserver.de
   ftp://ftp.myserver.de/shared
   ftp://192.168.0.21
   ftp://192.168.0.21/shared
   ```

5. The port specification `Port 21` is the standard port for the FTP protocol. Generally there's no need to change this. 

6. Remove the option `Passive Transfer Mode` if you want an active transfer. We find passive mode leads to less problems during the transfer.

7. If access is protected uncheck the option `Login anonymously` and enter your username and password.

8. Click on `Test FTP Server` to test the connection to the FTP server.

9. If the connection test was successful click on `OK`.


