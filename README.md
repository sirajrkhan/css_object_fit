#Business case for using CSS3 "object-fit:cover" property

#Optimizing the thumbnails for random pictures
A guide on how to display same-size thumbnails without distorting the image, losing the aspect-ratio or making the picture out-of-focus for random size pictures.

#Background:
A landing page needs to be built for a conference, wherein Speakers’ photographs (thumbnails) need to be displayed in a specific dimension – say, 100px by 100px.

#Problem Statement:
The photographs are of random size and orientation (landscape, portrait & square) and coming from an external source on which the application does not have any control. Therefore, following solutions will not work:
•	Cannot individually crop profile pictures to match the thumbnail place-holder DIVs
•	Cannot force-fit pictures as per the placeholder dimensions as it will distort the aspect ratio
•	Cannot dynamically mask the image either from top or center due to uncertain size

#Solution:
CSS3 property “object-fit: cover” comes to the rescue. It helps in maintaining the aspect ratio while filling the entire content box. The object size is resolved as a cover constraint against the container/images used width and height.

#Scope:
Did I tell you that it is working only on Chrome :)