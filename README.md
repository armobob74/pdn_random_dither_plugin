If you don't already have paint.NET, get it at https://www.getpaint.net/download.html

Download all files and run the installer. You should find the finished product available in paint.NET under Effects/Stylize/Random Dither. 

But what is random dithering anyways? Imagine that you want to process an image so that each pixel is either black or white. One approach you may consider 
is to loop through each pixel in the image and assign it to black or white depending on whether or not the pixel intensity is above some fixed threshold. 
Unfortunately, this method is likely to lead to an unacceptable loss of detail.

One clever way to improve this method is by using a random threshold for each pixel. When we do this, pixels in darker regions have a higher probability of coming out black,
and pixels in lighter regions have a higher probability of coming out white. This ends up translating a lot of detail over to the final result. 


Running a random dither almost feels like visualizing a probability space, which is why it's one of my favorite dithering algorithms. 
