===========================
Should you start a project?
===========================



Well, unless you want to quickly open an image and take a look at it, the answer is “almost always.” Some features will only work in projects, many scripts will only work in projects (as exported files and folders look specifically along the “project” file path). It will also allow you to quickly and uniformly apply your script/pipeline to a large set of images.
As of 0.2.0m3, some image types with multiple scenes or sub-files will only open in projects.

To start a project you will need an empty folder.

0.1.2+ - Use the Create project button in the Project tab, select your folder.

0.1.3+ - Drag an empty folder into the open QuPath window
Import images

I recommend placing the images you want to analyze within the project folder whenever possible. This makes the project as a whole more portable, as you can copy it onto the network, a USB drive, etc, and open it anywhere without disrupting the file path to the images.

0.1.2+ - Drag a single image into the QuPath window that has a project active. Or in the Project tab, click Import images which will allow you to navigate to the image location and select large numbers of images.

0.2.0m3+ - Select and drag large numbers of images into an open QuPath project. Requires a project to be open, follow the dialog instructions after.

Once you import an image, a project file (project.qpproj) will be generated in the project folder. Since I work with many projects, and in Windows, I find it useful to rename the project. Once it has been run (by double clicking it), it can be accessed more quickly by right clicking on the QuPath icon on the taskbar, which will then have it in the list of recently opened files.
image
image.png368×872 44.4 KB

It isn’t going to be quite so easy to figure out what all of those “project” projects were.

Project files themselves are the .qpproj file within the originally empty project folder. This is what you would run, or drag into an open QuPath window, or open through the file menu. The data files are stored in the “data” folder, and are named based on their association with an image file. They store all of the objects you see in the overlays (annotations, detections). If you are doing something destructive with your data, it is sometimes a good idea to back this folder up somewhere else so you can return to a previous step if you don’t like the results after a “Run for project.”

In 0.1.2/3 you will usually get a Scripts folder within the project if you save scripts in the default location (Automate->Project scripts). This function is broken for 0.2.0 through at least m4, and you will have to rely on setting a scripting directory for all of QuPath.

If you create a trained classifier, you will also get a “classifiers” folder.

Additional folders can be created (like the Images folder mentioned above) without interfering with the project itself, though I don’t recommend editing file names until you are comfortable with how the project works.

You now have a project and area ready to either learn more about how objects in QuPath work, or jump into your analysis.

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
