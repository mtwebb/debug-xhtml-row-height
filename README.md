# debug-xhtml-row-height
While working on an ebook version of a comic, I noticed the panels displayed correctly on the webpage, but incorrectly in the book page render.  The only difference between the files is the extension of the file (html for one and xhtml for the other). As can be seen in the screenshots below, the xhtml has <td> elems that have an additional 4 pixels beneath the image. This prevents the comic from reading as a single image.

Tested using Safari Webkit on Mac.

### goal: update css or html so the xhtml version of file matches the html one.
table.html renders correctly:
![html renders correctly](/readme/html.png)
table.xhtml renders incorrectly (note the 4 pixel gap between top and bottom row of images:
![xhtml renders incorectly](/readme/xhtml.png)

Is height not supported by XHTML?  Next test is to rebuild this using div, but appears to be the same.

