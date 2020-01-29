# The Basics

CONFIRE SHOWTIME consists of two parts: a Designer and a Player. The Designer creates and edits projects, the Player reads these projects and plays the  defined content on a display.

CONFIRE SHOWTIME is a decentralized system, it requires no central application server or central database. Even a functioning network is not a must (although this does make things easier).

## Projects

A SHOWTIME project is made of multiple elements:

* A project file with the file extension `.shtproj`
* An accompanying project folder that contains all resources embedded in the project

A project file is an XML file in which resources, layouts, showcases and schedules are defined.  Resources either point to embedded  files (stored in the project folder) or external files (held outside of the project)

## Project archive

A project in its original form isn't so easy to transport as it's not enough to just copy the XML project file. The corresponding project folder is needed too. For this reason there is the project archive.

A project archive is a Zip archive that stores all relevant project files in a compressed file. Project archives have the file extension `.shtarc` and can be easily copied or sent via email.

CONFIRE SHOWTIME DESIGNER can save any project as a project archive on request. Conversely it can import any archive as a project. CONFIRE SHOWTIME PLAYER can also open project archives directly.

It's worth nothing that project archives are also the publishing format for SHOWTIME projects, i.e. technically speaking whenever you publish a project with CONFIRE SHOWTIME a project archive is created.

## Resources

Resources are files, file groups, folders, text, playlists or database connections. Resources are the foundation level in the structural design of a project.

The following types of resources can be defined:

Type                | Description
------------------- | ---------
Graphics file        | PNG, JPEG, GIF or Bitmap file
Graphics collection   | A folder containing graphics files
Video file          | WebM or MP4 file
Video collection    | A folder of video files
Audio file          | WebM or MP3 file
Audio collection    | A folder of audio files
SVG file            | SVG file
HTML page           | A folder containing all files of an HTML website
PDF file            | PDF file
Text                | Markdown formatted text
Playlist            | Sequence of graphics, videos, audio, and/or PDF pages
JSON file          | JSON file
XML file           | XML file
CSV fil           | CSV file
Database connection | Database connection to MS Access, MS SQL Server, PostgreSQL, Firebird, MySQL or ODBC
Custom app          | Folder of HTML/CSS/Javascript files

There are two ways to embed file based resources:

* *Embedded Resources* are resources where the files belong to the project. Whenever you add an embedded resource the files are copied to a designated subfolder within the project folder. When you publish the project or save it as a project archive then these files are included in the publication of the project archive.

* *External Resources* are resources that are simply linked to by the project file. They are not copied into the project folder and are not affected or changed when publishing or creating a project archive. It is just important to note that the path to the files or folders in the network must be openly available. Generally, external resources are stored in a network folder and are addressable via UNC path (i.e. `\\MyServer\MyFolder`).

By default we advise you to embed your resources. Reasons to use external resources could be:

* You have files or folders which you'd like to change outside of the project. For example, file contents which change regularly. Changing an external resource has the huge advantage that it's then not necessary to republish the project.

* For large file sizes such a videos or high resolution pictures which could unnecessarily prolong publishing and subscribing.

* Files which need to be edited by a team who are not authorized to access the project.

Aditional formats can be integrated as a resource via conversion:

* Mircrosoft Office: Conversion of Word documents and PowerPoint presentations as a PDF resource.

* OpenOffice/LibreOffice: Conversion of Writer documents and Impress presentations as a PDF resource.

## Layouts

Layouts are design templates for Showcases which you will set up later. Layouts are arranged hierarchically beginning with a Master Layout. The Master Layout defines the resolution of the target screen (i.e. 1920 x 1080 pixels for full HD). You can add any number of Master Layouts to a project. A Master Layout can contain any number of sublayouts and each sublayout can in turn contain any number of further sublayouts. In each layout (Master Layout or Sublayout) you can create and position graphical elements.

Graphical elements can be positioned, rotated and resized via Drag & Drop. Other aspects such as color, transparency, font, background, borders and distances can be easily defined by the appropriate editors.

The following graphical elements are available:

### Picture

Picture elements visualize picture resources i.e. With this element you can display PNGs, JPEGs, GIFs or Bitmaps. 

### Text

Text elements visualize either text resources or text inputted directly. Using text resources you can use one and the same text within multiple text elements.

### Multimedia 

Multimedia elements visualize playlists. With these you can display a sequence of pictures, videos and/or PDF pages. With a playlist you can use one and the same sequence in multiple multimedia elements. 

### SVG   

SVG elements visualize SVG resources. With this element you can display vector-based graphics whose quality always remains the same regardless of the resolution. 

### Website

Website elements visualize either HTML resources or directly embedded URLs. You can also embed entire websites and allow or prevent interactivity.

### Shapes 

Shape elements are geometric elements without content. However, like any other element they also have a background and a frame. These are used for graphical support. For example, you can set the color and transparency of a specific layout area with a panel element.

### Apps

Apps are graphical elements with complex contents. We currently provide the following apps:

Name           | Description
-------------- | ---------
RSS Ticker     | Display messages and news feeds
Weather        | Weather forecasts
Uhr            | Time display
DAVINCI WEBBOX | Display DAVINCI timetables, substitution plans and floorplans

What's more you can also implement your own apps. For this you simply need knowledge of HTML/CSS/Javascript.

> We plan to bring you more apps in the future.

## Showcases and Scenes

Showcases define the time coordination of layouts in your presentation. All Showcases start with a Master Layout. Inside there is where the resolution of the target screen is defined. Within a Showcase you can create any number of scenes. A scene refers to just one layout of the layout hierarchy of the Master Layouts and defines the duration and transition of each layout. The result is a sequence of scenes. The total running time of all scenes is displayed by the Showcase duration.

By creating multiple Showcases each with their own  target resolution the content of all public displays can be managed in a single project. Layouts and resources and also be used together when needed. 

## Schedules

With schedules multiple Showcases can be synchronized from one project. It can even shut down the computer automatically at a specified time. For this we create time-activated tasks. An example of this could be at the moment the Player starts the project (where in this case the task is started immediately) or at a later time that can be defined by repeat time patterns (date, time as well as daily, weekly or monthly repeats). 

Each schedule can receive multiple subschedules. Each subschedule can in turn receive any number of subschedules. This allows tasks to be grouped in larger schedules.

The following tasks are available:

### Start Showcase

This task starts a Showcase presentation at a given time.

### Start schedule

This task start a subschedule at a given time. Only schedules relative to the schedule can be started in which the task is defined.

### Shutdown system

This task shuts down the computer. You can select whether to shutdown the computer completely, switch to standby mode or enter hibernation mode. Optionally you can specify whether to activate  Wake On Standby mode. This mode allows the computer to automatically start up again at a given time.

> #### info::Wake On Standby
>
> Wake On Stand By allows you to start up a computer that is in standby or powered off using its power built-in options. Here the computer is not entirely powered off but waiting in a special minimalized power mode and just able to react to a internal schedule. Not every computer supports this function as it's dependent on the hardware capabilities of the computer. Wake On Standby is not to be confused with Wake On LAN, a similar technology where an external network command triggers startup of the computer.

## Publish Projects

Once you've defined all Showcases and Schedules you can distribute your project to your public displays. The easiest way to do this is to publish a project.

CONFIRE SHOWTIME publishing means creating a project archive and then saving it in a designated location either in the local network or on the internet where one or more Players can access it. If all Players are available over the local network then it makes sense to publish the project in a network folder. If however your Players are distributed over multiple locations you can publish the project on the internet. For that you have several options:

* Publish to an FTP server
* Publish to a WebDAV server
* Publish to a Cloud Storage Service (DropBox, Microsoft OneDrive or Google Drive).

> #### primary::Tip
> 
> All Cloud Storage Services supported by CONFIRE SHOWTIME require a registered account in order to use their services. Use of these services is free up to a certain limit.

## Subscribe Projects

A Player subscribe to one or more projects. Subscribing means that the Player will check whether the project has changed at regular intervals. If this is the case it is downloaded to the computer of the public display and becomes available. If the subscribed project is currently being displayed it will automatically be exchanged. In other words: Subscribe just once to a project and all subsequent changes will be reflected without to do anything else to the public display
