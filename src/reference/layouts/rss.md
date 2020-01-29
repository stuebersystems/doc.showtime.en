# Using RSS

[RSS] is an XML format for saving news. RSS for reading is also referred to as RSS Feed. The RSS Ticker app from CONFIRE SHOWTIME can read and display these RSS Feeds. There are two possibilities:

1. You consume a public RSS Feed (for example from a news website)

2. Or you can create your own RSS Feed and publish your own news and messages.

## Create an RSS Feed

Proceed as follows:

1. Open the Windows Editor (or a different text editor) and create a new blank file.

2. Paste this XML text block in the Text Editor:
   
   ```` xml
   <?xml version="1.0" encoding="UTF-8" ?>
   <rss version="2.0">
     <channel>
       <title>My Messages</title>
       <item>
         <title>Graduation Party in the Auditorium</title>
         <description>There will be a graduation party in the auditorium today at 4:15pm.</description>
       </item>
       <item>
         <title>There will be no school tomorrow</title>
         <description>There will be no lesson at our school tomorrow.</description>
       </item>
     </channel>
   </rss>
   ````

3. Change the contents as you please. For additional entries, copy the item node as often as necessary.

4. Save the file in a network folder.

5. In the RSS Ticker element enter a file URL under `URL`. For example:
   
   ````
   file:///\\myserver\feeds\news.xml
   ````

You don't need to know anymore about RSS than that. If you still want to get a more detailed understanding of the RSS format we recommend the relevant chapter on [w3schools.com](http://www.w3schools.com/xml/xml_rss.asp).

## RSS Feed URLs

To embed an RSS feed in the RSS Ticker App you must enter a URL. With a URL you can not only point to web addresses but local files and files in the network too.

Example for a Web URL:

````
http://www.newsrss.bbc.co.uk/xml/rss2
````

Example for a local file:

````
file:///c:\feeds\news.xml
````

Example for a file in the local network:

````
file:///\\myserver\feeds\news.xml
````

[RSS]: ../../simple-glossary.md#rss