JAVMovieScraper
===============

JAVMovieScraper is a Java Swing program to scrape English XBMC metadata for Japanese Adult Videos (JAV) found on JavLibrary.com and DMM.co.jp.

As no one site has a complete set of English metadata, the program amalgamates metadeta info from a variety of sources, including dmm.co.jp, javlibrary.com, squareplus.co.jp, and actionjav.com
The data is then fed through a machine translation (if original data is in Japanese) and then quality checked to sanitize it and poster elements are cropped so only the cover is shown.

This program is in alpha. Please submit bugs and feature requests here on github on the issues page!

###### Usage

1. Make sure you have the Java JRE installed. You will need at least Java version 7. Java can be downloaded here: https://www.java.com/en/download/index.jsp
2. Either compile the source yourself or download and run the precompiled JAR from her: http://www.mediafire.com/download/pm3d2yl49qa99fe/JAVMovieScraper.jar
3. Initially, the program will load your home directory in the file pane on the left. Click the open directory button below this file list and point it to the directory where your movie file you wish to scrape is.
4. Select the movie file in the list of files. Your movie file MUST have the JAV ID as the last word within the filename, not including stacked file indicators such as DISC1 or CD1. The JAV ID can be optionally surrounded by brackets or parenthesis and can contain a dash before the numerical part. Examples of OK file names: My Movie - ABC-123, My Movie - [ABC123] CD1, ABC-123, (ABC-123)
5. Click either the "Scrape (Automatic)" button or the "Scrape" button on the bottom part of the program. Scrape (Automatic) will work 99% of the time, but if you get the wrong result when scraping, try using "Scrape" instead to manually specify which URL to use when scraping dmm.co.jp. It's also worth trying "Scrape" if actor images are not appearing.
6. After a little while, the metadeta for the movie will appear in the editor pane. You can select one of the several titles found using the drop down list, or edit the entry by typing in your own text.
7. When you are happy with the way the metadata looks, click the "Write File Data" button to create the poster,fanart and nfo files for your movie. Note that for now, not all metadata downloaded is shown in the editor, but this data IS written to the nfo file.
8. If your file wasn't already in its own directory, you can click the "MovieToNewFolder" button to move the nfo, poster, movie files, and fanart to a new folder. If the movie file was only named by the ID name (e.g. ABC-123), then the title of the movie was be automatically appended to the folder name.


In the future I intend to add batch processing modes and command line options.