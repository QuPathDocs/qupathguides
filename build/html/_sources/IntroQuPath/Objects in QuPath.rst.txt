
Objects in QuPath
^^^^^^^^^^^^^^^^^
Images in QuPath are not modified, basically ever, but data objects of two general types are created, annotations, and detections. These objects are not “burned in” to the image, but are instead visualized as an overlay. The objects themselves contain data relevant to the pixels “below” them.

Annotations are intended as large, generally simple, structures and have measurements that update automatically as they are changed. This makes them slower to render and handle in terms of analysis, and having many annotations or highly detailed annotations (with a lot of vertices) can lead to massive slowdowns. Detections are generally smaller, simple objects that are not structurally modifiable, but the rigidity of their data means the program can support many more of them. These are general rules, and there are exceptions. Spots, for example, are annotations.

Overall, ~99% of projects will involve creating one or more Annotation objects, and then generating further Detection objects within them. Those Detections will then be classified or measured in some way in order to produce a general number (% positive), which can then be saved in the “parent” annotation object. A list of annotation measurements across a variety of images can then be generated for a summary at the end of a project. The simplest example would be a list of image names that each had a single annotation, with the percentage of positive cells as the primary statistic of interest.

Ready to get started? Or skip to the end and learn how to generate summary data for your project?

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
