========
Versions
========

Which version should I use?


There are currently 2 main variants available for download here 2:
0.1.2

is the current stable release, and probably the best one to get started with. Most publications use this version. It does require the BioFormats package and extension for many file types 6. If your files do not open, the first thing to check is whether you have BioFormats correctly installed.
0.1.3 (doesn’t really exist) has some significant improvements over 1.2 in certain areas (positive pixel detection, drag and drop folders for projects), but requires building it yourself using Gradle (more details here in Pete’s blog if you want to pursue this).

Projects in 0.1.2 and 0.1.3 are mostly compatible. There is a hard break with all projects in 0.2.0m1 and above.
0.2.0m#

The newer, possibly less stable versions (they are mostly fine :slight_smile: ). They have significantly improved features, but not everything is working. It doesn’t require BioFormats to be added separately (built in, and in fact attempting to add BioFormats can break it), but does have a few in progress features that either are not scriptable or are not entirely working. Use with caution, not a great idea for long term projects unless you need particular features as they will likely not be forward or backwards compatible. Even between m# versions, as you might see if you try to certain scripts from m2 in m3 :slight_smile:

M4 Out now! More details here: https://petebankhead.github.io/qupath/2019/08/20/fourth-milestone.html
Warning:

If you use m2, the projects are far less mobile as fixed file paths were used, as opposed to relative file paths. That means that even if you stored the images within the project folder, you couldn’t move the project folder to another computer/drive/location without editing the text file, see here for an example.

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
