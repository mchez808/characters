# Pillow

This tutorial is taken from Kenneth Love, Python instructor at [Treehouse](https://teamtreehouse.com).  Treehouse has been my top resource for learning and practicing not only Python, but VCS using Git, Bash commands, and computer science courses such as algorithms and data structures.  I can't recommend it highly enough!

Pillow is the successor to PIL, the Python Imaging Library.

[Pillow documention](http://pillow.readthedocs.org/)

[External libraries installation guide](http://pillow.readthedocs.org/en/latest/installation.html#external-libraries)
. These are libraries you may need to install before you can open up specific image types on your computer.




## Common terms and methods

`Image`

- Class for accessing images.

`.open(path)` 

- Open an image for manipulation

`.rotate(angle, resample=0, expand=0)`

- Rotate an image by angle degrees. If you set expand to True, the resulting image will be big enough to view the entire original image.

`.resize(size, resample=0)`

- Resize an image to the width and height specified in a tuple like (500, 500).

`.thumbnail(size, resample=1)`

- Resize an image so it fits within the width and height provided in the size tuple. thumbnail changes the Image instance and doesn't return a new image.

`.copy()`

- Copies the image to a new variable.

`.crop(box=None)`

- Cuts out the specified box from the image. The box is a tuple of four numbers in the following format: (left, top, right, bottom).

`.save(file, format=None, **params)`

- Save the Image to a new or existing file name or file object. format lets you override the format of the image.

`.paste(image, box=None, mode=None)`

- Pastes an Image into another Image. The pasted region must fit totally within the bounds of the pasted-into Image. It'll be placed into the provided box.

`.transpose(method)`

- Let's you apply some preset rotations and reflections to images.


