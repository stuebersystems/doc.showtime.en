# CONFIRE SHOWTIME Documentation

This is the English documentation for CONFIRE SHOWTIME. The documentation is Open Source and we have implemented it using [GitBook](https://github.com/GitbookIO/gitbook).

> ## Important information:
> The open source version of GitBook used here is no longer under active development. The current version of GitBook is not open source. 

## Install GitBook for Windows

1. [Install node.js](https://nodejs.org/de/download). Node.js includes allready the package manager npm.

2. Launch the installer and follow the on-screen instructions.

3. Run the command prompt as Administrator.

4. Enter the command `npm install gitbook-cli -g` to install a local copy of GitBook.

## Clone Repository

This repository is a Git repository. To clone the repository to a local commputer you will need a Git client. Either install [Git for Windows](https://gitforwindows.org/) and use the command prompt or install one of the many GUIs. We recommend [GitHub Desktop](https://desktop.github.com) or [SourceTree](https://www.sourcetreeapp.com).

1. Create a local directory for the documentation e.g. `c:\docs\showtime`.

2. Open the command prompt and change to directory `c:\docs\showtime`.

3. Enter the command `git clone https://github.com/stuebersystems/doc.showtime.en.git` to clone the repository.

## Download Repository as Zip Archive

If you don't want to use Git you can even download the repository as a Zip Archive:

1. Open the URL `https://github.com/stuebersystems/doc.showtime.en` in your web browser

2. Click on the `Clone or download` button then select `Download ZIP`.

3. Extract the Zip Archive to a local folder, e.g. `c:\docs\showtime`.

## Using GitBook

You have installed node.js and the GitBook package, cloned the repository or downloaded it as a Zip Archive. Now you can generate the documentation locally on your computer:

1. Start the command prompt and change to the directory `c:\docs\showtime\src`.

2. First you have to install all needed GitBook plugins. Enter the command `gitbook install`. GitBook plugins will be installed. This needs to be done only once for this documentation.

3. Enter the command `gitbook build`. CONFIRE SHOWTIME documentation will be regenerated.

4. To display the result, change the folder to `c:\docs\showtime\src\_book` and open the file `index.html` in your webbrowser.

The table of contents can be found in the `SUMMARY.md` file. 

## Further Informationen

+ [Git - All you need to know](https://git-scm.com/book/en/v2)
+ [GitBook on GitHub](https://github.com/GitbookIO/gitbook)
