# Linux_basics

# Navigation
Linux filesystems are based on a directory tree. This means that you can create directories (or “folders”) inside other directories, and files can exist in any directory.

To see what directory you are currently active in:

```pwd```
This stands for “print working directory”, and will print the path to your current directory. The output can look similar to this:

```/home/foo```
This means that your current active directory is foo, which is inside home, which lives in the root directory, /.

To see other files and directories that exist in your current working directory:

```ls```
This will give you a list of names of files and directories. To navigate into a directory, use its name:

```cd <name of directory>```
This will change your new current working directory to the directory you specified. You can see this with ```pwd```.

Additionally, you can specify .. to change to the directory one level up in your path. To get back to your original directory:

```cd ..```
We can also create new directories in our current working directory. For example, to create a new directory called bar:

```mkdir bar```
Then we can

```cd```
into bar if we want. We can also delete bar if we no longer find it useful:
```rm -d bar```
```rm -d```
will only delete empty directories.
# File Manipulation
Files cannot be used with

```cd```
(it stands for “change directory”).
Instead, we can view files. Say we have a file baz in our current directory:

```cat baz```
This will print out the entire contents of baz to the terminal.

With long files, this is impractical and unreadable. To paginate the output:

```less baz```
This will also print the contents of baz, but one terminal page at a time, beginning at the start of the file.

Use the spacebar to advance a page, or the arrow keys to go up and down one line at a time. Press q to quit out of less.

To create a new file called foobar:

```touch foobar```
This creates an empty file with the name foobar in your current working directory. The contents of this file are empty.

If we decide foobar isn’t such a good name after all, we can rename foobar to fizzbuzz:

```mv foobar fizzbuzz```
```mv```
stands for “move” and it can move a file or directory from one place to another.
By specifying the original file, we can “move” it to a new location in the current working directory, thereby renaming it.

It is also possible to copy a file to a new location. If we want to bring back foobar, but keep fizzbuzz too:

```cp fizzbuzz foobar```
Just as you guessed,

```cp```
is short for “copy”. By copying fizzbuzz to a new file called foobar, we have replicated the original file in a new file with a different name.
However, what good is a file if it contains nothing? To edit files, a file editor is necessary.

There are many options for file editors, all created by professionals for daily use. Such editors include vim, emacs, nano, and pico.

nano is a perfectly suitable option for beginners. It is easy and simple to use, with no bells or whistles to confuse the average user.

To edit text into foobar:

```nano foobar```
This will open up a space where you can immediately start typing to edit foobar.

To save the written text, press

```Ctrl-X```
then y. This returns you to the shell with a newly saved foobar file.
Now foobar has some text to view when using

```cat```
or
```less```
.
Finally, to delete the empty fizzbuzz:

```rm fizzbuzz```
Unlike directories, files are deleted whether they contain content or not.






Markdown basics:
# Parragraph 
> # Dependencies
> Run the command line below:
>
> >```sudo apt-get install freeglut3-dev```
# How to make a list:
1. Clonar el repositorio y abra la terminal desde el folder ***src/Calibration***.
2. Ejecute el comando: 
```make```
3. Cuando termine de construir ejecute: 
# Titles
## Pasos para la compilación, calibración y ejecución
### Calibración y ejecución

# Insert code
```/src/Calibration/Image/```

# Insert photos
![title](cal.PNG)

# Bold and italic
***src***

# Parragraph and code
>> ```cv::aruco::detectMarkers(image, dictionary, corners, ids);```
