//====================================================================================================

Launching

npm i

Developer mode. npm run dev command
Production mode. npm run build command
Production mode and sending the result to the server via FTP. npm run deploy command
Production mode and creating a ZIP archive with the result. npm run zip command
Production mode without creating WEBP images and actions related to this format. npm run devbuild command

//====================================================================================================

Architecture

The package.json file is a file containing commands for launching builders, information about installed plugins and their versions (can be edited if necessary). As well as other information about the author and version of the template.

The gulpfile.js file is the main GULP builder file. Contains connections for various tasks and scenarios for their execution (can be edited if necessary)

The snnipets.txt file is a file with snippets that are used when working with a template. 

README.txt file - brief information on working with the template

File cover.jpg - Black Sea Fleet cover

The config folder contains folders and files for configuring the work of collectors, as well as files with individual tasks.

src folder - contains project source files and folders.

//====================================================================================================

The contents of the config folder:

The gulp-settings.js file — contains settings for paths to files and folders for GULP work, as well as settings for an FTP connection for uploading results to the server

The gulp-plugins.js file is an auxiliary file that contains the connection and export of a list of common plugins for GULP tasks

The file webpack.dev.js — contains the configuration of WEBPACK work in developer mode

The file webpack.prod.js — contains the configuration of WEBPACK work in production mode

folder gulp-tasks — contains files of individual GULP tasks

//====================================================================================================

Contents of the src folder:

favicon.ico file - site icon

The index.html file is an index page-content, it is not automatically updated when editing (if you want to delete it)

The home.html file is the main page of the site (if you wish, rename it to index.html)

Files folder (empty) - all files from this folder will be copied to the result folder (dist/files)

svgicons folder (empty) - used to create the SVG sprite

The html folder contains .HTM files that are included in the HTML files of the pages (for example, in home.html). Here you can create your own plugins.

scss folder - contains site style files and folders

js folder - contains files and folders of site scripts

The img folder is where the pictures of the project are stored. Initially, only a cover photo of the template

//====================================================================================================

The contents of the src/html folder:

Files from this folder are intended for inclusion in HTML-files of pages.

The _header.htm file is preparation for creating the site header. Contains a <header> tag and a bounding box. Initially included in home.html

The _footer.htm file is preparation for creating a site footer. Contains a <footer> tag and a bounding box. Initially included in home.html

The _head.htm file contains the <head> tag inside which meta tags are indicated, the site icon is connected, the style file, and the <title> tag with the title variable. Initially included in home.html

The _js.htm file is intended for connecting common js files. Contains the connection of the main js/app.min.js file from the result. Initially included in home.html

The _popup.htm file is preparation for creating popups. Contains boilerplate, commented out HTML code. Initially included in home.html.

The _pagging.htm file is preparation for creating a paging navigation block. Contains boilerplate HTML code.

//====================================================================================================

The contents of the src/scss folder:

The style.scss file is the main stylesheet. Contains various settings and connections of other files.

The home.scss file is the style sheet for the home page. Initially empty and included in style.scss

The header.scss file is the site header style file. Contains the commented code for the burger menu button. Initially included in style.scss

The footer.scss file is the site footer style file. Initially empty and included in style.scss

The common.scss file is a style sheet for common, reusable blocks in a particular project. Initially empty and included in style.scss

The base.scss file is a file of basic styles of the Black and White template. Contains useful SCSS templates and commented connection files with basic styles of various modules.

The libs folder contains files of complete (factory) styles of various modules and plugins

The fonts folder contains the style file(s) associated with the fonts. Contains the icons.scss file to connect the icon font.

The base folder contains auxiliary files of B&W styles, as well as files with basic styles of various models. For convenience, module files of the same group (for example, form elements) are collected in separate subfolders. There is also a file with zeroing styles null.scss

//====================================================================================================

The contents of the src/js folder:

The app.js file is the main script file. It serves to connect the functionality and other settings required in the project.

The libs folder — contains files of ready-made additions, as a rule, not intended for editing.

The files folder contains files of various modules and other functionality.

The contents of the src/js/files folder:

The script.js file is designed to write your own code for the project. Initially imported in app.js

The functions.js file contains small modules and various auxiliary functionality. Initially imported in app.js, but modules are commented out

The gallery.js file contains the plugin connection and gallery styles. Initially imported into app.js, commented out. If necessary, you can make changes to it.

The sliders.js file contains the plugin connection and slider styles, functionality for automatically adding classes, code for creating specific sliders. Initially imported into app.js, commented out.

The tippy.js file — contains the plug-in connection and tips plugin styles. Originally imported into app.js, commented out.

The map.js file (in progress) contains template code for implementing map functionality.

The modules.js file is an auxiliary file for the work of the ChF.

The forms folder contains files of modules for working with forms

The scroll folder contains modules for working with site scrolling