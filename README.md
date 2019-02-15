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

Line 18:

- This line opens a body tag, which is where the bulk of all
  your html code will go.  This tag is much more tangible than
  the head tag, as almost everything in the body tag will be
  viewable in the final product.
