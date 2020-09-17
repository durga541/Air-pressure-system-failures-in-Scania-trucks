# Air-pressure-system-failures-in-Scania-trucks
The main purpose of this project is to classify the failures of the Scania trucks is whether by the components
related to APS (Air pressure system) or by the other components that are not related to APS. The data has
only 2 classes i.e. positive or negative. So, this is a binary classification problem.
There is also misclassification cost associated with this problem.
 
 pred  act_pos   act_neg
 pos      -       Cost_1
 neg    Cost_2      -

Here, Cost_1 refers to the cost that an unnecessary check needs to be done by a mechanic at the workshop
and Cost_1 is 10, while Cost_2 refer to the cost of missing a faulty truck, which may cause a breakdown
and Cost_2 is 500.
Total_cost = Cost_1 x No_Instances + Cost_2 x No_Instances.
Here, our goal is to minimize the total cost by reducing the errors especially type 2 errors i.e false negatives.
