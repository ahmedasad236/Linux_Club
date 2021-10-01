# Ranger

**What is ranger?**

Ranger is a small and efficient console-based file manager with VI key bindings, it comes with a minimalistic interface displaying the directory hierarchy allowing you to quickly navigate through different files.

**Ranger features:**

Common file operations such as copy, delete, create, etc…

Renaming multiple files at once

Uses rifle ( a file launcher that determines automatically which programs to use for each type of files)

Tabs, Bookmarks, Mouse support

Multi-column display

UTF-8 Support

Preview of the selected file/directory.

VIM-like console

**Installing ranger:**

Ubuntu/Debian

              $ sudo apt install ranger

CentOs

              $ sudo yum install ranger 

Arch Linux

              $ sudo pacman -S ranger

**Starting ranger:**

               $ ranger

**Useage:**

Appearance: The first column shows the parent directory, the second is the main column and the third column shows a preview of the current file/directory.

Navigation: using arrows or (h j k l)

Open a file: Enter 

Close (quitting) a file: q 

**Optional Dependencies:**

To enable the file preview of images and videos, we need to install the following dependencies :
w3mimgdisplay or ueberzug  for images previewsffmpegthumbnailer  for video thumbnailspdftoppm bb          to preview of PDF

Installation:

On Ubuntu/Debian 

                   $ sudo apt-get install ueberzug ffmpegthumbnailer  poppler-utils

On Arch Linux

                    $ sudo pacman -S  ueberzug ffmpegthumbnailer poppler

**For more information about ranger:**

                    $ man ranger