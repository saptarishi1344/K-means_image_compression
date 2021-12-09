# K-means_image_compression
compress image using K-means algorithm


Algorithm:
first we read the image and convert it into a 2D array.
Then we initialize clusters with their center pointing to random locations
Then we find out the euclidian distance of each point from all the centers, and find out the minimum
then we assign those pixels and replace with values in the centers
we convert the image back to its 3D form

Pseudo-code:

Import necessary libraries.
Define function to read image and return an image with smaller intensity values for easier calculation
Next function we convert the image, since it is a color image from 3D matrix to 2D matrix using np.reshape() function, this makes the clustering algorithm simpler and faster
in the same function we randomly initialize the means(centroid array) with random x, y values.
in the next function we have a nested loop to go through all the points of the image, as well as to go through the cluster centers to check for the minimum distance, and update the points belonging to the clusters accordingly,
this entire thing is again iterated for 10 times, to update the average(centroid of the image)
Next we have a function for converting the image back into its 3D form.
