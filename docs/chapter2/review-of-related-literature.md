# Review of Related Literature

Studies that dealt with the implementation of traffic related systems
were reviewed in order to support the current study.

The first related study is entitled "Real-time Traffic Congestion Detection Based on Video Analysis"
by Shan Hu, Jiansheng Wu, Ling Xu <sup>1</sup>. In this study real-time
video analysis is done to detect traffic congestion on a particular road. While density of vehicles is the main
factor used in the detection of traffic congestion it also includes the velocity of moving vehicles.
Both are fed into the fuzzy logic algorithm to determine the road's condition.
Fuzzy logic is used in the research because of its nature. There are no clear boundaries
on what defines a traffic congestion (e.g A slow flow of vehicles does not mean it is experiencing heavy traffic).
This uncertainty behavior found on traffic situations makes fuzzy logic based systems suitable.
The current study is similar to the related study specifically on the use of density and vehicles velocity as
inputs to the fuzzy logic algorithm for traffic congestion detection.
It makes use of OpenCV (Open Source Computer Vision Library)
to perform background difference and perform morphological operation.
OpenCV is used for the detection process of the vehicles in the proposed system.
On the other hand, the current study extends beyond traffic congestion detection since it also includes notification.

The second study is entitled "Traffic Simulation System Based on Fuzzy Logic" by Mohammad A. Taha and Laheeb Ibrahim <sup>2</sup>.
In this study, a traffic simulator which uses a fuzzy logic engine to compare and review results is developed.
Their system has a graphical user interface to physically see the intersection and simulate traffic from there. It
also included a graphical user interface for the fuzzy logic engine to manipulate input, output and fuzzy rules. The
system is tested using a variety of test cases which simulate traffic and its behavior. The fuzzy logic engine and fixed
time controller were compared and it was found out that traffic flow on the fuzzy logic controlled traffic showed better results.
The current study is similar to the related study on the use of the fuzzy logic algorithm, however, the former is only limited
to traffic congestion detection and will not go into traffic simulation.

The third study that is reviewed is entitled "An Intelligent Traffic Controller Based on Fuzzy Logic" by Bilal Ahmed Khan and
Nai Shyan Lai <sup>3</sup>. Fuzzy logic concepts and image processing techniques using OpenCV are utilized in this study.
The simulated environment is controlled through a Peripheral Interface Controller (PIC) micro-controller which controls traffic signals
in a desired manner. Fuzzy logic is used in this related study to prolong the green phase depending on the traffic flow. The actual
fuzzy logic instructions are found in the micro-controller itself making it an autonomous system. The Fuzzy logic controller
now receives the number of detected vehicles from the vision sensor with extract data and produces a unique output for each
scenario. The fuzzy logic design consists of six membership functions namely; zero, few, fewer, more, much and numerous.
`If else` statements are used to perform relationships between the membership functions and defined 30 rules for
possible scenarios for each traffic signal. The current study is similar to the related study on the uitilization of the
fuzzy logic algorithm, however the current study won't control traffic, but rather, notify registered users using SMS to
avoid traffic congested roads.

---

<sup>1</sup> Shan Hu, Jiansheng Wu, Ling Xu (2012), 9: 10,  2907–2914, "Real-time Traffic Congestion Detection Based on Video Analysis"  
Retrieved from http://www.joics.com/publishedpapers/2012_9_10_2907_2914.pdf  
Viewed: June 16, 2015  

<sup>2</sup> Mohammad A. Taha and Laheeb Ibrahim (2012), 12, 356–360, "Traffic Simulation System Based on Fuzzy Logic"  
Retrieved from http://www.sciencedirect.com/science/article/pii/S1877050912006758/pdf?md5=72a355f021b2ef8eebc01a7c9649feee&pid=1-s2.0-S1877050912006758-main.pdf
Viewed: July 11, 2015  

<sup>3</sup> Bilal Ahmed Khan and Nai Shyan Lai, 89-93, "An Intelligent Traffic Controller Based on Fuzzy Logic"  
Retrieved from http://sdiwc.net/digital-library/download.php?id=00000573.pdf
Viewed: July 11, 2015  
