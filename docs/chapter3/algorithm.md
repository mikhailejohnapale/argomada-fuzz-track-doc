# Fuzz Logic

The study uses fuzzy logic to provide an output for the Traffic Congestion Notification System.
Contrary to binary logic, fuzzy logic provides truth values ranging from 0 to 1 inclusive since 
this logic deals with approximate rather than fixed and exact reasoning.

In the figure above, a temperature can be both cool and cold at the same time.The ranges 0 to 1 
is the degree of membership of how cool and how cold a temperature might be, the range is also 
called a grade or  a level. Cold, Cool and Hot are  called liguistic variables,  they represent 
the value of a temperature in words. Another term in fuzzy logic is the Membership function,wherein
“input data are group into sets”(e.g T(temperature)={cold,cool,hot}).By having a membership function,
an input value can have multiple sets (e.g cool  0.3 and cold  0.7 at the same time) with different 
degree of membership. Membership functions can be grouped to create a fuzzy set(see Figure 2).

Label is used to name each membership function. A seven membership function can be labeled as: NL 
(negative large),NM (negative medium),NS (negative small), ZR (zero),PS (positive small),PM 
(positive medium),PL (positive large).

Another process of fuzzy logic  is defining the rules that will establish a relationship between the
input value and the output value , this is called inferencing process.  The input is necessary to 
activate the rules and only if it satifies the IF part of the rule statement.

Figure 3 shows that rule 1 is activated when the two fuzzy sets' inputs have satisfied the given rules. 
The defined rules is also called Fuzzy rules.
Figure 4 shows  an example of a rules translated to a table for easy understanding. The rules relates 
speed and density inputs to  traffic congestion status output.  The evaluation of fuzzy rules and its 
results is possible  through fuzzy set operations. These operations are needed in order to obtain a final
result from fuzzy sets   that will be used in defuzzification process.


Defuzzification, is the final process of fuzzy logic where an output is obtained from the overall result 
of the fuzzy sets.

Here are the two most common method:
1. Maximum Value Method
The maximum value method  bases the final output value on the rule output with the highest membership 
function grade.

2.Center of Gravity Method
The center of gravity method, also referred to as “calculating the centroid,” mathematically obtains 
the center of mass of the triggered output membership functions. In mathematical terms, a centroid is 
the point in a geometrical figure whose coordinates equal the average of all the other points comprising 
the figure.

where:
Output data = the number of counts to be used for the output
FO  = the fuzzy output in counts for labels n = A through G
FGrade  = the fuzzy grade level for levels n = A through G

In conclusion these are the main processes of fuzz logic algorithm: fuzification,inference and 
defuzification. 

Fuzification
1. Defining the linguistic variables.
2. Construct membership functions.
3. Contruct fuzzy rules.
4. Convert input into fuzzy values.
Inference
1. Evaluate the fuzzy  rules.
Defuzification
1. Use one of the defuzzification methods to come up with an crisp output   or non-fuzzy values.
