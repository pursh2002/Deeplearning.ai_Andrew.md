 # Basic Neural Net work: Binary Classification 
 [https://en.wikipedia.org/wiki/Binary_classification
 
 ## Logistic Regression
 
 1 cat vs  0 non cat 
 
 * image representation in a computer [https://en.wikipedia.org/wiki/Classification_rule
 
 three matricis red/green/blue 
 
 if image is 64 * 64 pixil
 
 then the three matricis red/blue/green represent 64*64*3 = 12288
 
n = nx = 12288 

x(input image) ----- (Predict) y == 1 or 0

(x,y) y e {0,1}

m train example : {x(1),y(1)},{x(2),y(2)}.....{x(m),y(m)}

m=m(train)    m=m(test)

[ ] matrix

python X.shape = (nx,m)


same apples to y = [y1,y2.....ym]
y.shape=(1,m)

#### Sensitivity and specificity https://en.wikipedia.org/wiki/Sensitivity_and_specificity
Sensitivity and specificity are statistical measures of the performance of a binary classification test, also known in statistics as classification function:

Sensitivity (also called the true positive rate, the recall, or probability of detection[1] in some fields) measures the proportion of positives that are correctly identified as such (e.g. the percentage of sick people who are correctly identified as having the condition).
Specificity (also called the true negative rate) measures the proportion of negatives that are correctly identified as such (e.g. the percentage of healthy people who are correctly identified as not having the condition).
 
 
* a false positive (detecting a disease when it is not present) is considered differently from a false negative (not detecting a disease when it is present).

# [https://en.wikipedia.org/wiki/Precision_and_recall

# Logestic regression

given x want y^ = P(y =1|x) 

x = nx dimension vector

parameters : w = nx,b= the number

how do we generate output y^=   sigmid(wTx + b)
if z larger sig = 1
if z small sig = 0
sigmoid=1/1+e
Y^ = 0<y<1
