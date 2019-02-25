SRC Folder Breakdown

The following is an analysis of all the files and folders in
the root of the SRC directory.

-------------------------------------------------------------

- The first sub-folder in SRC is the DOC folder, short for
  Documentation.  Simply put, this folder is where you put
  all files related to the documentation of the template.
- The second sub-folder is the IMG folder, which is short for
  image.  As you may have guess, any assets having to do with
  images are stored here.
- The final sub-folder we have in SRC is JS, which stands for 
  JavaScript.  This is where all JavaScript files and assets 
  are stored.
- The first file we have in src is .EditorConfig.  This file
  is used to maintain consistent text formatting in collaborative
  projects.  The file is simply a list of settings to be used 
  by each coder's IDE.
- The next file we have is the .GitAttributes file.  This file
  is created and used by the Git VCS.  This file lists off if
  each file extension in the project will be converted to a 
  text format or left as binary.
- Next we have the .GitIgnore file.  This is another file used
  by Git.  As the name would suggest, the .GitIgnore file lists
  the files and/or directories that are to be left untracked
  by Git.  Useful if you have a todo list or other non-critical
  files.
- The next file we have is the first one that is used in the actual
  web template.  404.html is a standard 404 page, used when a user 
  tries to access a page that doesn't exist (usually as a result of
  broken links).
- BrowserConfig.xml is a file that's only used under certain 
  circumstances, specifically if the page is accessed using 
  Internet Explorer 11 running on Windows 8.  In that case it
  is used to create the background images and colors of the page
  but is otherwise optional.
- FavIcon.ico has two traditional uses.  The first is as the 
  small icon that appears next to the site in your bookmarks 
  list.  The second use is almost identical, except that instead
  of appearing in your bookmarks list it appears in the address bar/tab 
  header of your browser.
- Humans.txt is a short file designed to give proper credits to
  the team responsible for the project.  All they need to do is 
  put their names and roles in the file.
- Icon.png is a slightly larger version of favicon.ico, and is 
  used as the Apple Touch Icon in the event that the program 
  becomes an app.  This would be the icon you tap to start the
  app.
- Index.html is the default landing page for the website, and 
  most likely the first page the user will see.  A more detailed
  explanation of this file will be included in the next section.
- Robots.txt is used in regards to webcrawlers from search engines
  like Google.  Specifically it is used to determine whether
  certain pages of the website are allowed to be index by crawlers,
  or if the crawlers are disallowed from doing so.
- Site.WebManifest is a short manifest of the contents of the
  website stored as a .JSON file.  The main things stored in 
  the file are the name, author, icon, and description.
- Tile.png is similar to Icon.png, but instead of being used 
  as a touch icon for an app, it is used as the icon when you
  pin the program in a Windows environment.
- Tile-wide.png is virtually identical in purpose to the prior
  file, the only functional difference being a higher resolution.
  This one is used for the "windows" display in Windows 10.
  
--------------------------------------------------------------

Index.html Breakdown

This section will go over each line of the index.html page.

-------------------------------------------------------------

Line 1:

- This line is referred to as a doctype declaration, which is
  effectively a set of instructions given to the browser to let
  it know what version of html must be used.

Line 2:

- This line opens the HTML tag, which the entire page will be 
  enclosed in.  This tag allows for certain variables to be set,
  such as 'no-js.'
- This code is used for interfacing with Modernizr, a JS plugin
  for browsers.  If Modernizr is running, it replaces the 'no-js'
  with 'js,' allowing JavaScript to be run.
  
Line 4:

- This line opens a Head tag, which is the place to store meta-
data and declare any links to external files.

Line 5:

- This is an example of a meta-data tag, which allows for many
  different options to be set.
- This line sets the encoding system to UTF-8, which is the 
  preferred encoding scheme for online applications.  Encoding
  in this case refers to how the data is encoded into binary.
- It's very important to declare this as soon as possible in
  this file, otherwise you're vulnerable to data breaches and 
  hijacking due to unencoded data being left vulnerable.
- UTF-8 is the modern equivelant of the ASCII encoding scheme,
  and is fully backwards-compatible with ASCII.  It is also very
  widely used and thus encoding a website in UTF-8 ensures maximum
  compatibility.

Line 6:

- This meta-data tag is enabling another option, more
  specifically enabling support for older versions of 
  Internet Explorer.  The line "ie=edge" will tell Internet
  Explorer to display the page in the most recent IE format
  It can support, usually IE9.
  
Line 7:

- This line open and closes an empty title tag.  Title tags
  are used to display the name of the website/web page in the
  tab of the browser.
  
Line 8:

- This line establishes the page's meta-description information,
  which is often used in search engine results.  The only time
  this description is seen by a user is as the description of
  the web page when it appears as a result of a search.  If
  this is left blank, the search result description will be
  taken from the first paragraph of the page.
  
Line 9:

- This line is called the viewport meta-tag, and is used to 
  help scale a website down to fit on a mobile device screen.
  A manual width can be set, or the width can be set to match
  the device's screen.  An optional scaling factor can be set
  to further adjust the mobile display.
  
Line 11:

- This is an example of a link tag.  The 'rel' field determines
  how that document relates to the current one, and the 'href'
  field denotes the url or filepath for that document.
- In this case, the tag is denoting that the specified file
  is this page's manifest file.
  
Line 12:

- This line specifies what image is the app's Touch Icon,
  which we covered earlier.
  
Line 13:

- This line is an example of a comment.  Comments are not
  read or executed when the rest of the code runs and usually
  serve to exist as notations on an app's code for other
  programmers to read.
  
Line 15:

- This is a link to an external style sheet that will be used
  to format the web page. Using external style sheets is considered
  good practice since you only need to change one file instead of
  every linked page.
  
Line 16:

- This is another link to an external style sheet.  Multiple
  style sheets can be utilized to pull off different effects.

Line 17: 
- This line closes the previously opened head tag, making sure
  that anything past this point is not treated as part of the 
  head tag.  Always close your tags.

Line 19:

- This line opens a body tag, which is where the bulk of all
  your html code will go.  This tag is much more tangible than
  the head tag, as almost everything in the body tag will be
  viewable in the final product.
  
Line 20:

- This comment appears to be designed to interface with Modernizr,
  specifically the browser detection feature.  This line will
  execute if modernizr detects that the user is using an old
  version of Internet Explorer and display a message suggesting
  an upgrade.

Line 21:

- This line begins with a paragraph tag, configured to the
  type of "browserupgrade."  Most HTML tags can be set to sub-
  types in order to alter their behavior in some way.
- This line continues with plain text that spells out the 
  desired message.  Within this line of plain text are formatting
  tags, such as < strong > to indicate boldface.
- This line also has an integrated hyperlink to redirect the 
  user to another webpage if they click on it.
  
Line 22:

- This line appears to close the if statement that was opened
  in the previous comment.

Line 24:

- This comment exists to give instruction on how to modify 
  it for the programmer's use.
  
Line 25:

- This is another paragraph tag with more plain text.

Line 26:

- This is an example of a script tag.  Instead of writing JavaScript
  in the HTML file, you can link an external JavaScript file
  instead.  This is the recommended method.  The SRC field is used
  to denote the location of the external JS file.
- This JS tag is calling the main JS file for Modernizr.  At
  this point when the code is executed, the linked file will be
  called and carry out its function, so be sure to place your
  JS tags after the code you want it to work on--or, ideally, at
  the end of the entire file.
  
Line 27:

- This Script tag is linked to an external JQuery website for
  added functionality.  The "integrity" and "crossorigin" fields
  are added security measures.  Integrity is denoted to specify
  what protocol to go with if the original source of this script
  has been manipulated in some way, and likewise the crossorigin
  is used to specify what to do when the source file is hosted
  on a different server.
  
Line 28:

- This script tag is an example of an in-line JavaScript code.
  Functionally this will work just as fine as calling an external
  file.
- This is a particularly interesting JavaScript line because
  it's calling a JQuery function in the current window, which
  also calls and executes a second JQuery function.
  
Line 29&30:

- These two lines link additional JS files from the JS folder
  in this project.
  
Line 32:

- This is another comment with instructions for the programmer.

Line 33:

- This line opens a Script tag.  The following lines are another
  way to do in-line JS.
  
Line 34&35:

- These lines are actual JS code, which has entirely different
  formatting and syntax than html.  These two lines contain
  multiple JS statements separated by ;
- What these lines do is prepare and send a Google Analytics
  tracker with information about your website.  This is a very
  good tool to track various post-production and usage statistics
  about your website.
  
Line 36:

- This line closes the previous Script tag, an important step.

Line 37:

- This is another Script tag, but with the inclusion of Async
  and Defer, it will run after the entire web page has been loaded
  and will even effect the lines below it.

Line 38:

- Closes the body tag.  You'd get serious errors without this.

Line 40:

- Closes the html tag, ending the file.
  You'd get serious errors without this.
  
------------------------------------------------------------
1.	1958: Bell Labs creates the modem
2.	1969: Arpanet is founded.
a.	 Arpanet was a military computer network that was used for sharing data long distance. It was developed under ARPA and soon linked four different universities computers together. ARPANET would send information by using packets. The basis for the internet can be traced back to ARPANET
3.	1971: Ray Tomlinson sends the first network email
a.	  Ray Tomlinson sent the first email using a software called “SNDMSG.” He also introduced the “@” symbol to separate the person name and location. Tomlinson sent the first email to a colleague in the same room as him, to check if the software was working properly. To this day, the message within the email has been forgotten. 
4.	1974: TCP/IP ideas are introduced in a protocol for packet network intercommunication.
a.	  Vinton Cerf and Robert Kahn published A Protocol for Packet Network Intercommunication. Because many of the existing computers operated on its on hardware and software, it became almost impossible for computers to commutate to each other. Cerf and Kahn created a protocol, TCP, that allowed cross networking. They published their network architecture in May of 1974. 
5.	1974: the word Internet is coined
a.	  In Internet Transmission Control Program, internet is first used in the acronym IP, which stands for Internet Protocol. 
6.	1983: ARPANET adopts TCP/IP 
a.	  ARPANET scientist began to assemble the “network of networks” that became the modern
7.	1984: Domain Name System (DNS) is introduced
a.	  Paul Mockapetris recognized one problem with ARPANET’s problem with translating addresses into a single table on a single host. He introduced DNS and it become a one of the internet standards n the IETF. Some of the DNS include: .com, .gov and .edu. 
8.	1990: HTML language is created. 
a.	  Developed by Tim Berners-Lee, HTML was used to create web pages, that could be displayed on the WWW. Without the creation of HTML, web pages would not be able to correctly display text or images. 
9.	1990: The World Wide Web (WWW) is introduced. 
a.	   Tim Berners-Lee and his team developed the WWW as a way for scientists in universities and institutes around the world to share information. The first ever website is: http://info.cern.ch/
10.	1991:  http://info.cern.ch/
a.	   Tim Berners-Lee publishes the first ever website, http://info.cern.ch/. It describes how the web works and how to use it.
11.	1993: Mosaic is created and becomes the first popular web browser. 
a.	   Marc Andreessen and Eric Bina designed Mosaic for Windows. Funding was provided for the project and the first alpha release was published in June 1993. It was not until September 1993 that the first beta was released. 
12.	1994: WebCrawler is the first full search engine 
a.	   Brian Pinkerton first created WebCrawler at the University of Washington. WebCrawler was only used as a desktop application. In April 1994, the search engine had over 4,000 websites. By November 1994, it hit its one millionth search query. WebCrawler is the oldest surviving search engine and is still in operation. 
13.	1994: Amazon is founded
a.	   Jeff Bezos created Amazon in July of 1994. It original started as an online bookstore. The company is now worth ~$1 trillion. 
14.	1995: DOT-COM BOOM BEGINS
15.	1995: Apache is created 
a.	   In 1994, Brian Behlendorf and Cliff Skolnick created a group of developers to create Apache. After testing out the many enhancements and bug fixes to the NCSA base, they released their owned server, Apache, was released in April 1995. It became the most widely server. It is free to use and download. 
16.	1995: Java is created
a.	   James Gosling, Mike Sheridan, and Patrick Naughton started working on the java project in 1991 and was initially used for television. It was released in 1995 under Sun Microsystems Java platform. Java was a key component in the internet. Java code was designed to have less implementation dependencies and to run on all platforms that supported Java. 



