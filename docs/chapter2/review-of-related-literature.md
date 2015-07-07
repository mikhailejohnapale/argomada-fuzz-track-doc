# Review of Related Literature

The researchers reviewed and studied similar implementations of traffic related systems
in order to design and implement the proposed traffic detection system. The studies below
are reviewed and scrutinized thoroughly.

The first related study is entitled "Real-time Traffic Congestion Detection Based on Video Analysis"
by Shan Hu, Jiansheng Wu, Ling Xu <sup>1</sup>. In this study the researchers proposed a method using real-time
video analysis to detect traffic congestion on a particular road. Density of vehicles is an important
factor in detection of traffic congestion. The procedure to detect density of vehicles are: 1) Frame
difference of moving vehicles 2) Lane detection based on accumulating vehicles moving locus. Next detection
process is the detection of moving vehicles itself. The algorithm to detect the moving vehicles are the
following; 1) Change the RGB image to gray image; 2) Subtract the two adjacent frames; 3) Employ the
median filter to get rid of noise points; 4) Check the difference result to get a binary image;
5) Apply morphological operation and fill region of vehicles. The researchers does not stop on vehicle detection. They have
also included the vehicles velocity and optical flow model which will be used in fuzzy logic to determine
the roads condition. Fuzzy logic is used in the research because of its nature. There is no clear boundaries
on what defines a traffic congestion (e.g A slow flow of vehicles does not mean it is experiencing heavy traffic),
this uncertainty behavior found on traffic situations makes fuzzy logic based systems suitable.
The proposed system has similar procedures regarding the detection of traffic congestion.
The proposed system will use OpenCV (Open Source Computer Vision Library) 
to perform background difference using background subtraction function which is used to create blobs in
the image and perform morphological operation to remove noise from the image. After the noise is removed,
it can contour the remaining blobs and mark them as objects of interest which are vehicles in the image.
OpenCV library is the leading open source computer vision and machine learning software library that
that has more than 2500 optimized algorithms to recognize objects and motion in consecutive images <sup>2</sup>.
OpenCV is used for heavy-lifting the detection process of the vehicles in the proposed system. 


---

<sup>1</sup> "Real-time Traffic Congestion Detection Based on Video Analysis"
Source: http://www.joics.com/publishedpapers/2012_9_10_2907_2914.pdf Viewed: June 16, 2015

<sup>2</sup> "About OpenCV"  
Source: http://opencv.org/about.html Viewed: July 7, 2015