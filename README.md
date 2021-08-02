# Resize-Images
Code to resize images for the web

This will take a folder full of images taken with, say your phone, optimize them for the web and place the resized images in a folder called 'web/' located inside the existing folder. The original images will not be altered.

You can then upload the optimized images to your website.

You have to change the path to the point to the folder on your machine.

You can change the size of the resized images, for example the code resizes landscape images to 3264px by 2448px. You can change these values on lines 36, 40 and 44 (depending on landscape, portrait or square) to suit your own requirements.

On line 18 we have "im = ImageOps.exif_transpose(im)". Mobile phones don't know which way is up, so a picture you take that you think is landscape can end up being portrait. Smart phones have an accelerometer which writes the orientation into the images metadata. So this line attempts to check which way the picture should be oriented. Be warned, this does not always work, so Photoshoppery may be required.

Once you have your folder path and target size sorted, you can then run the code. I open the code in Visual Studio Code and run the code by pressing Ctrl+Alt+N. You will need the Python extension loaded.# Resize-Images

Make sure the Python script and all images are installed on your local machine. The code wont work if you point to a remote path such as Dropbox.
