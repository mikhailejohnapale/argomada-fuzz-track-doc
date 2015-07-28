#Fuzzy Logic

   The study uses fuzzy logic to provide an output for the Traffic Congestion 
Notification System.Contrary to binary logic, fuzzy logic provides truth 
values ranging from 0 to 1 inclusive since this logic deals with approximate
rather than fixed and exact reasoning. The main processes of fuzzy logic 
algorithm are  fuzzification,inference and defuzzification. 

###Fuzzification###

* Define the linguistic variables.
   Linguistic variables are variables in the fuzzy logic  system which 
represent the input variables in words rather than numbers.( e.g low , moderate , high )
* Construct membership functions.
   Membership function, wherein input data are group into sets(e.g V(velocity)={low,moderate,high}).
By having a membership function, an input value can have multiple sets (e.g low  0.3 and moderate 
0.7 at the same time) with different degree of membership. Membership functions can be grouped to 
create a fuzzy set(see Figure 2).
   The grade or level  are ranges 0 to 1 inclusive identifies the degree of membership of an input. 
Label is used to name each membership function. A seven membership function can be labeled as:
NL (negative large),NM (negative medium),NS (negative small), ZR (zero),PS (positive small),
PM (positive medium),PL (positive large).
    

* Construct fuzzy rules.
   Another process of fuzzy logic  is defining the rules that will establish a relationship
between the input value and the output value. 


* Convert input into fuzzy values.
   An input is converted into fuzzy values using the membership functions by   assigning its 
degree of membership to a particular membership function.

    The figure above shows an input of 0.4 velocity has a fuzzy value of 0.7 in slow membership  
and 0.3 in medium membership.

###Inference###

   The process of inference evaluates the fuzzy rules. When the necessary input is given it 
will activate the  rules and only if it satifies the IF part of the rule statement.

    Figure 4 shows  an example of a rules translated to a table for easy understanding.
The rules relates speed and density inputs to  traffic congestion status output.  
The evaluation of fuzzy rules and its results is possible  through fuzzy set operations. 
These operations are needed in order to obtain a final result from fuzzy sets   that will 
be used in defuzzification process.

###Defuzzification###

    **Defuzzification**, is the final process of fuzzy logic where an output is obtained from 
the overall result of the fuzzy sets. 
Here are the two most common method:

1. Maximum Value Method
        The maximum value method  bases the final output value on the rule output with the highest
     membership function grade.

2.Center of Gravity Method
        The center of gravity method, also referred to as “calculating the centroid,” mathematically 
    obtains the center of mass of the triggered output membership functions. In mathematical terms, 
    a centroid is the point in a geometrical figure whose coordinates equal the average of all the other 
    points comprising the figure.


    where:
    Output data = the number of counts to be used for the output
    FO  = the fuzzy output in counts for labels n = A through G
    FGrade  = the fuzzy grade level for levels n = A through G
