Download Link: https://assignmentchef.com/product/solved-computer-vision-lab-session-no-4
<br>
<h1></h1>




The following items are the steps that you have to do in this lab session:




<h2>Color-based segmentation</h2>




<ol>

 <li>Display the 6 images in grayscale and split them in the three RGB channels and in the three HSV channels.</li>

 <li>Note the variation of the RGB components and of the Hue one in the area of the dark car that turns on the left for the 6 images.</li>

 <li>Select in the image “ur_c_s_03a_01_L_0376.png” the area corresponding to the dark car that turns on the left, e.g. area [390:400,575:595]. In this area compute the mean value (<em>m</em>) and the standard deviation (<em>s</em>) of the Hue component.</li>

 <li>Segment the dark car in the 6 images by thresholding the Hue component (e.g. in the range between <em>m-s</em> and <em>m+s</em>).</li>

 <li>Display (i) the binary images corresponding to the segmentation and the related centroid and bounding box; (ii) the centroid and bounding box overlapped on the color image (tips: <em>regionprops()</em> function needs a logical matrix; display the bounding box of the blob with the highest area; see Fig.1).</li>

 <li>Repeat the steps 2-5 for the red car on the street (tips: to chose the corresponding area; hue range &gt;0.97 and &lt;1 (why?); to try the hue range between <em>m-s</em> and <em>m+s</em>).</li>

</ol>




<h2>Blob detection</h2>

<ul>

 <li>Compute the Laplacian responses for the two highlighted sunflowers in Fig.2 and show them as a function of the scales. Then, compute the characteristic scale (and its value in pixels) for the two selected objects. Tips: see slides 34-35; see <em>m</em>; parameters: starting standard deviation 1, number of scales 10, standard deviation increment sigma=1.5*sigma.</li>

</ul>




<strong>Notes: </strong>

<ul>

 <li>You have to write a report that describes your work and the obtained results (please include the figures). In the report you must indicate all the surnames of the participants (not other names, e.g. the teachers).</li>

 <li>About the code:

  <ul>

   <li>You have to use relative paths.</li>

   <li>You have to write and use functions.</li>

   <li>You have to provide us a main script to test your code.</li>

  </ul></li>

 <li>The code must be uploaded as M-files. All the files (M-files, images, and report) have to be compressed in a single file named “surnames_labxx.zip/tgz” (all the surnames of the participants have to be indicated), and then the compressed file has to be uploaded.</li>

</ul>







detected object




detected object

1000          1200                                                 200            400            600            800           1000         1200










detected object




<table>

 <tbody>

  <tr>

   <td width="320"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

detected object

1000          1200                                                   200            400            600            800           1000         1200







Fig.1: Segmentation examples.
















Fig.2: Sunflowers.