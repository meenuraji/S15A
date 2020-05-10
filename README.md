# S15A


Data set of 100 backgroung images of streets and roads

https://drive.google.com/open?id=1r6nffKopmf7CpLJUCiQG4jMNDxryQ17i

Background images were downloaded and resized to 224* 224 uing GIMP 

Image

!Image(

Data set of 100 foreground images of cars
https://drive.google.com/open?id=1n82xIWQGfcnz4DnYbkIjgwbW4l_kbL1x
car images were downloaded, backgrounds were deleted uing 3Dpaint and car images with tranparent background were created. *Regreted this step in later stages of creating depth images- as it created blur margins

Image

Data set of 100 foreground masks
Tried using 3Dpaint and GIMP for creating masks of foreground images Image

Data set of 300k overlay images of fg on bg
https://drive.google.com/open?id=1c8tO4rYzJtpDFUu5bJ0XBE9uvtl6ZWzH

Image

300k Masks of overlayed images
https://drive.google.com/open?id=1og3tDEszR1N6lqEZsc6DE3s-9EG3cfzp
Image

Depth estimation of 300k overlay images
https://drive.google.com/open?id=1JUupNIBdN-oZdGwyctPhyzOPpKqO3_86
Tried the Depth model reference given (https://github.com/ialhashim/DenseDepth/blob/master/DenseDepth.ipynb) and with few modifications able to implement nyu-h5 on the overlay bg-fg images.
Depth predictions were not prominent. Tried other options for better predictions. Tried KITTI ICCV (https://github.com/nianticlabs/monodepth2) and foundout better depth predictions than nyu-h5. My intusion for poor depth prediction of few fg images is (*As menctioned erlier) becaue of poor selection of foregroung images i.e with some what blur margins

Image
