# Review of Related Literature

The researchers reviewed and studied similar implementations of traffic related systems
in order to design and implement the proposed traffic detection system. The studies below
are reviewed and scrutinized thoroughly.

The first related study is entitled "Real-time Traffic Congestion Detection Based on Video Analysis"
by Shan Hu, Jiansheng Wu, Ling Xu. In this study the researchers proposed a method using real-time
video analysis to detect traffic congestion on a particular road. Density of vehicles is an important
factor in detection of traffic congestion. The procedure to detect density of vehicles are: 1) Frame
difference of moving vehicles 2) Lane detection based on accumulating vehicles moving locus. Next detection
process is the detection of moving vehicles itself. The algorithm to detect the moving vehicles are the
following; 1) Change the RGB image to gray image; 2) Subtract the two adjacent frames; 3) Employ the
median filter to get rid of noise points; 4) Check the difference result to get a binary image;
5) Apply morphological operation and fill region of vehicles;