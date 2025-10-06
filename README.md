# v6.2.1
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Fixed an issue with the zoom feature

# v6.2.0
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Upgraded few dependencies

# v6.1.1
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Added a `nospaces` transformation for [TEXT] prefix
* Fixed an issue with the N-Up task not handling correctly pages with `null` content

# v6.0.2
*  Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Fixed an edge case with the rotation tool when multiple files are selected
* Added Dutch translation
* Added Polish translation

# v6.0.1
* Upgraded Electron
* Upgraded PDF engine
* Fixed an edge case of the fonts subsetting in the Compress task
* Fixed an edge case of the Resize task when CropBox and MediaBox are not the same

# v6.0.0
* Added N-up tool to arranges multiple pages of a document onto a single page
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Fixed Portuguese locale for menus
* Fixed an issue with some tools not asking for the password for encrypted documents
* Fixed the context menu to customize file names that wasn't always setting the correct string

# v5.5.2
* Upgraded Electron
* Upgraded PDF engine
* Fixed a duplicate entry in the "Continue with" menu
* Fixed English locale on MacOS

# v5.5.1
* Upgraded Electron
* Fixed an issue with drag and drop of files

# v5.5.0
* Upgraded Electron
* Upgraded PDF engine
* Fixed an issue with optional content and compress task

# v5.4.1
* Upgraded Electron
* Applied workaround for `.deb` package on Ubuntu 24.04 https://github.com/electron/electron/issues/42510

# v5.4.0
* Upgraded Electron
* Upgraded PDF engine
  
# v5.3.2
* Upgraded Electron
* Upgraded PDF engine
* Fixed an issue with the compression task that was adding a black background to compressed images in some corner case

# v5.3.1
* Upgraded Electron
  
# v5.3.0
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine

# v5.2.0
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Fixed an issue with the locale detection that was setting the application to German on the first run

# v5.1.0
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Fixed an issue where some menus weren't properly localized
* Added pages count to Split By Text

# v5.0.1
* Upgraded Electron
* Better menu for the placeholders suggestions
* `[TEXT]` and `[IMAGE_NAME]` placeholders are less restrictive regarding invalid chars
* Improved grayscale conversion

# v5.0.0
* Added a task to Extract images from PDF files. The task can use the `[IMAGE_NAME]` placeholder to drive the name of the generated files.
* Added a task to convert pages of PDF files to images (PNG, JPEG, TIFF)
* Added a task to flatten form fields and page content
* `[IMAGE_NAME]` and `[TEXT]` placeholders can optionally be piped with string transformations. Ex. `[TEXT | upper], [TEXT | lower], [TEXT | capitalize], [TEXT | replace('this', 'that')], [TEXT | upper | replace('this', 'that')]`
* Compress task now subsets TrueType fonts
* Page normalization in Merge tool is now a combo with an additional entry
* Show skipped files, if any, when the user selects "Skip existing files"
* All the menus are now localized
* Some of the tasks option fields are now persistent (automatically save/restored)
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine

# v4.3.1
* Upgraded Electron
* Fixed a couple of cosmetic issues

# v4.3.0
* Upgraded Electron to the next maintained major version
* Added Korean language

# v4.2.1
* Upgraded Electron

# v4.2.0
* Upgraded Electron to the next maintained major version
* Added an icon to hide/unhide password fields
* Added a dark theme

# v4.1.1
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Upgraded Electron

# v4.1.0
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Upgraded Electron to the next maintained major version
* Proper Tiling patterns streams processing in the Compress task

# v4.0.5
* Fixed an issue handling files with multiple lines of garbage on top

# v4.0.4
* Upgraded Electron
* Upgraded PDF engine
* Offline activation tokens now use anonymized username
* Failing tasks now show the PDF file that was processing and failed
* Improved handling of broken PDF files where the PDF engine has to perform a full scan of the PDF objects
* We now handle correctly those files containing garbage bytes at the beginning

# v4.0.3
* Upgraded Electron
* Fixed a proxy authentication issue

# v4.0.2
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Fixed an issue with the Normalize page size in the Merge tool where outline and link annotation destinations may end up with wrong destination coordinates
* Fixed an issue with the Resize tool where outline and link annotation destinations may end up with wrong destination coordinates
* Fixed an issue with Tiling patterns streams that weren't processed during the optimization process. This could lead to missing pattern resources in some cases
* Expected output file extension is automatically added when missing

# v4.0.1
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Added support for SVG, WebP, Multiple TIF and AVIF to the ImagesToPdf tool
* Added support for SVG, WebP, Multiple TIF and AVIF to the Organize pages tool
* Added support for SVG, WebP, Multiple TIF and AVIF to the Merge PDF tool
* Added tab navigation focusing the images and page thumbnails
* Added `alt + p` shortcut to open the preview of the focused element
* `SPACE` key now selects the focused element
* Closing the preview will focus the original page/image 
* Organize pages tool: add blank pages made more usable and fixed few edge cases

# v4.0.0
* Upgraded Electron
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Added a _Resize pages_ tool
* Replaced the pages magnifier with a button to open a page preview with additional zooming power
* New dashboard with "Tools" and "Recent files"
* Restyled menu with Tools always at hand
* Added the number of expected output files in the _Split_ task
* _Visual Combine & Reorder_ task renamed to _Organize pages_
* Added the number of expected pages in the _Organize pages_ task
* _Organize pages_ now allows images input (jpg, png..)
* _Organize pages_ can now drag and drop files in between pages
* _Organize pages_ fixed an issue with the generated bookmarks tree
* _Images to PDF_ can now drag and drop files in between other files
* Proper handling of Exif rotation when an image is used as input
* _Delete PDF pages_ now allows to select all blank pages in one click
* _Extract PDF pages_ now allows to select all non blank pages in one click
* Proper MacOS menu with standard entries
* Simplified handling of "Overwrite output" in case of a single file output
* Added a setting to select the unit of measure as Inches or Centimeters, used in Crop and few other tools
* Crop now shows the crop area size
* In _Delete pages_ is now possible to set all pages for deletion in one click and then unselect those to keep

# v3.0.13
* Upgraded PDF Engine
* Upgraded PDF render engine

# v3.0.12
* Upgraded PDF Engine
* Fixed a corner case in Split and Extract pages tasks
* 
# v3.0.11
* Fixed an issue with the Encrypt tool and numeric passwords starting with `0`

# v3.0.10
* Upgraded PDF Engine
* Fixed an issue with the Compress task and softmasks defined in ExtGState
* Fixed an issue with the Combine and Reorder task that could lead to the task failing

# v3.0.9
* Upgraded Electron
* Upgraded PDF engine
* Added images rotation capabilities to the ImagesToPdf tool
* Correct handling of file names containing double quotes

# v3.0.8
* Upgraded Electron
* Upgraded PDF Engine

# v3.0.7
* Added check boxes to the Compress task to drive `Discard Bookmarks` and `Discard Multimedia`
* Upgraded PDF engine

# v3.0.6
* Fixed an issue with the validation of an Offline Activation Token
* Upgraded Electron

# v3.0.5
* Fixed D&D in Combine and Reorder
* Restored working buttons to Open file and Open Folder in task result modal

# v3.0.4
* Added drag and drop support to Mix, Merge, Images to PDF and Visual combine to allow dropping of files even after the first drop
* Fixed "please wait" modal window that was hanging sometimes on Windows

# v3.0.3
* Fixed ToC generation in Merge task to properly handle links pointing to rotated pages
* Fixed manual D&D sorting in Images to PDF task
* Merge, Mix, Images to PDF tasks now have a toolbar to add files and sort the input
* Updated PDF engine

# v3.0.2
* Fixed failure to start on Windows when `REG QUERY HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Cryptography /v MachineGuid` throws an error because of disabled permissions

# v3.0.1
* Fixed --clean argument that wasn't always working
* Proper support for JPEG2000 in compress task
* Upgraded Electron

# v3.0.0
* Added a Compress task to reduce files size
* Added a ImagesToPdf task to convert images to a PDF file
* Added buttons to quickly open PDF files generated by a tool with another tool (Ex. Merge and then Compress and then Encrypt)
* Added a setting to select the tool to load when the application starts
* Added a setting to set the default working directory where all the Browse buttons will open by default
* Added full screen support
* Display TIFF files preview in Merge module instead of a placeholder image
* Tasks options panel can now be closed by clicking outside the panel
* Added optional offline validation
* Upgraded Electron
* Upgraded PDF render engine

# v2.1.7
* Fixed Open folder button that wasn't always working
* Clicking Open folder or Open file now opens in foreground

# v2.1.6
* Fixed an issue in case of user permissions don't allow a REG QUERY on Windows

# v2.1.5
* Upgraded PDF Engine

# v2.1.4
* Extract pages task can now generate a separate PDF file for each selected  page set
* Improved merge of AcroForms to cover cases of more complex form fields hierarchies
* Fixed an issue where [antivirus software interfere with writing output files](https://github.com/torakiki/sejda/issues/375)
* Fixed a regression where Merge and Alternate Mix where not handling encrypted PDF files
* Upgraded PDF engine
* Notarization of the MacOS package

# v2.1.3
* Fixed the existing output policy setting that was always recognized as `RENAME`
* Fixed an issue where split tasks where generating big output in case of input PDF files not conforming the PDF spec
* Fixed the extract pages task in case of multiple input and an invalid page selection for one of the inputs
* `Customize result names` field automatically save/restore its value
* Upgraded PDF engine
* Upgraded Electron

# v2.1.2
* Handle # and % chars in filename
* Fixed merge task in case of images input only
* Handle bookmarks in non conforming PDF files generated by wkhtmltopdf
* Better handling of problematic chars in filenames when [BOOKMARK_NAME] placeholder is used
* Upgraded PDF engine
* Upgraded Electron

# v2.1.1
* Merge tool can now merge images (png, tiff, jpeg, bmp, gif) together with PDF files
* Better feedback in case of existing output file and FAIL as output policy
* Added an option to automatically populate the output field with the parent directory of the selected PDF file
* Added a context menu to most of the tools, to allow the user to quickly set the output field same as one of the input files
* Handling of special chars in Split by bookmarks -> Bookmarks containing text field
* Added a --clean command line argument to clear user preferences and license key
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Upgraded Electron

# v2.0.4
* Upgraded PDF engine
* Extract text doesn't fail in case of a batch extraction and one file of the batch doesn't have any text
* Added 32-bits bundles for Windows
    
# v2.0.3
* Fixed an issue with UNC paths on Windows

# v2.0.2
* Delete pages task to signal show an error when run with no pages left
* Added a `CTRL + d` shortcut to remove pages selection
* Better handling of UNC paths on Windows
* Updated translations
* Upgraded PDF engine
* Upgraded PDF rendering engine

# v2.0.1
* Moved env variable to system space. Added a USER_LICENSE_KEY to the MSI properties to install the license key as a user env variable
* Added `[TOTAL_FILESNUMBER]` to the possible prefixes
* Updated German translation

# v2.0.0
* Added Delete pages task
* Added Convert to grayscale task
* Added Extract text task
* Added Repair task
* New application look
* Rotate task can now be used on multiple input PDF files
* Upgraded PDF engine
* Upgraded PDF rendering engine
* Localization completely reviewed and updated
* Diminished the overall size of the application
* Added button to open the generated PDF file using the native PDF reader
* Improved user interface for the Extract pages task
* Added a `Discard bookmarks` option to Extract pages, Split by size, Split by bookmarks, Split by text
* Improved user interface for the Rotate task
* Added merge option to consider the first file as a cover when generating a ToC
* Improved user interface for the Crop pages task
* Added `Ends with` field to split by text
* Improved user interface for the Split task
* Added manual proxy configuration to the settings panel
* Language combo to properly show the default language
* Encrypted passwords for PDF file when saving  tasks parameters to output file
* Added a number of keyboard shortcuts
* Fixed split by text selection when moving among pages with `Next` and `Prev` buttons
* Fixed enabling and disabling (first page, last page) of `Next` and `Prev` buttons in split by text
* Added a Log Viewer window to show application errors
* Added MSI properties `LOCALE`, `ACCEPT_EULA` and  `BUGS_AUTOREPORT`
* MSI now installs env variables in user space and removes them on uninstall
* Added a .zip portable bundle

# v1.1.8
* Fixes bug in Encrypt task

# v1.1.7
* Updates PDF engine.
* Fixed a permission issue on Linux.

# v1.1.6
* Updates PDF engine.
* Updates EULA.

# v1.1.5
* Adds support for porxy configuration.
* Updates underlying PDF library.

# v1.1.4
* Adds Italian translation.
* Adds Spanish translation.
* Adds German translation.

# v1.1.3
* Moves config location on Windows from %USERPROFILE% to %APPDATA%.
* Updates Encrypt task adding more permissions.
* Updates underlying PDF library, includes many minor bug fixes.
* Fixes bug related to handling different files with the same name.
* Adds Portuguese translation.
* Remembers customised result filenames.

# v1.1.2
* Fixes bug related to activating the product

# v1.1.1
* Natural sorting of filenames (1.pdf, 2.pdf, 10.pdf, 11.pdf) for merge and combine & reorder tasks.
* Larger magnifier zoom (8x).
* Batch (multiple files) support for the Split by pages task
* Smaller bugfixes and improvements.

# v1.1.0
* Visual page composer for combining and reordering PDF pages
* Select file or folder output location, for each task
* After trial ends PDFsam Visual is free to use within daily limits. Upgrade for premium features and unlimited use.
* Various bug fixes and improvements

# v1.0.9
* Improves French translation

# v1.0.8
* Adds French language support

# v1.0.7
*  Minor fixes and improvements, updates credits section.

# v1.0.6
*  Fixes a critical bug that can lead to missing data.
*  Upgrades the PDF engine with various bug fixes and enhancements 

# v1.0.5
* Includes bugfix for pre-activated silent installs in enterprise environments

# v1.0.4
* 14-day trial
* Includes various bugfixes for existing tasks

# v1.0.2
* Includes various bugfixes for existing tasks.
* Adds support for pre-activated silent installs in enterprise environments.
* Added context menu to easily select, unselect, invert selection

# v1.0.1
* Improved size of smaller monitors
* Fixed permissions related failures.
* Improved combine and reorder task with multiple page drag and drop, simpler page delete.
* Filename patterns are now remembered.
* Fixed bug related to filenames with accented characters on Windows, other Windows related stability improvements.
* Better handling of large files, increased available memory pool to 1Gb.
* Upgraded sejda-console

# v1.0.0
* Added Split by text task
* Upgraded PDFjs with corrected cmaps folder
* Upgraded sejda-console
* Upgraded icons
* Fixed the encrypt task failing with AES256
* Hide purchase menu item for PRO users

# v0.9.2
* Added Crop
* Added rotation to the Combine and Reorder task
* Added a scroll to top tag
