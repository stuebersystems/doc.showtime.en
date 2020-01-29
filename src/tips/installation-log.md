# Create An Installation Log

Should you experience difficulties during the installation of CONFIRE SHOWTIME it's recommended you create an installation log (setup log). This is a text file that logs every step of the installation.

1. Copy the installer file (`confireshowtime64.msi` or `confireshowtime32.msi`) to a folder of your choice.

2. Open the Windows command prompt and enter the following command:
   
   ````
   msiexec /i "C:\Setups\confireshowtime64.msi" /L*V "C:\Setups\showtime.log"
   ````
   
   These are of course just example paths which you will need to modify for your installation.
   
3. Confirm with `[Enter]`. The will installation start.

4. Now follow the familiar on-screen instructions of the wizard. If the installation is ended premeturely the option `Show Log` will appear.
   
   ![Option to displaz the log](../../images/setup-log.png)

5. Tick this option and click on `Finish`. The Windows Editor will now open and show you the installation log.

You can now send this log file to our [Support Team] so that we can assist you in resolving the problem.

> #### Info::Hint
> 
> The CONFIRE SHOWTIME installer is based on  Windows Installer technology. This provides a runtime environment (msiexec) in which the MSI package can be executed.

[Support Team]: http://showtime.stueber.de/support.php