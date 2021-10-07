# Task_2 practice

> Before you create project files, use the mkdir command with brace expansion to create
empty project planning documents in the **/home/student/Documents/project_plans**
directory. (**Hint: if ~/Documents does not exist, the -p option for the mkdir command will
create it.**)

> Create two empty files in the **~/Documents/project_plans** directory:
**season1_project_plan.odf and season2_project_plan.odf**.

> Create a total of 12 files with names **tv_seasonX_episodeY.ogg**. Replace X with the
season number and Y with that season's episode, for two seasons of six episodes each.

> As the author of a successful series of mystery novels, your next bestseller's
chapters are being edited for publishing. Create a total of eight files with names
**mystery_chapterX.odf**. Replace X with the numbers 1 through 8

> Use a single command to create two subdirectories named **season1** and **season2** under the
**Videos** directory, to organize the TV episodes.

> Move the appropriate TV episodes into the season subdirectories. Use only two commands,
specifying destinations using relative syntax.

> Create a 2-level directory hierarchy with a single command to organize the mystery book
chapters. Create **my_bestseller** under the **Documents** directory, and **chapters** under
the new **my_bestseller** directory.

> Create three more subdirectories directly under the **my_bestseller** directory using a single
command. Name these subdirectories **editor**, **changes**, and **vacation**. 

>  Change to the **chapters** directory. Using the tilde **(~)** home directory shortcut to specify
the source files, move all book chapters to the chapters directory, which is now your current
directory. What is the simplest syntax to specify the destination directory?

> You sent the first two chapters to the **editor** for review. Move only those two chapters to the
**editor** directory to avoid modifying them during the review. Starting from the chapters
subdirectory, use brace expansion with a range to specify the chapter file names to move and
a relative path for the destination directory.

> While on **vacation** you intend to write chapters 7 and 8. Use a single command to move
the files from the chapters directory to the **vacation** directory. Specify the chapter file
names using brace expansion with a list of strings and without using wildcard characters.

> Change your working directory to **~/Videos/season2**, and then copy the first episode of
the season to the **vacation** directory.

> Use a single cd command to change from your working directory to the **~/Documents/
my_bestseller/vacation** directory. List its files. Use the previous working directory
argument to return to the **season2** directory.  From the **season2** directory, copy the episode 2 file into the vacation
directory. Use the shortcut again to return to the vacation directory.

> The authors of chapters 5 and 6 want to experiment with possible changes. Copy both files
from the **~/Documents/my_bestseller**chapters directory to the **~/Documents/my_bestseller/changes** directory to prevent these changes from modifying original files.
Navigate to the **~/Documents/my_bestseller** directory. Use square-bracket pattern
matching to specify which chapter numbers to match in the filename argument of the cp
command.

> After further review, you decide that the plot changes are not necessary. Delete the **changes**
directory.

> When the **vacation** is over, the **vacation** directory is no longer needed. Delete it using the
**rm** command with the recursive option.