# Pattern-discovery-Datamining

implement the Apriori algorithm and apply it to mine frequent itemsets from a large dataset.

## Input
The provided input file ("categories.txt") consists of the category lists of 77,185 places in the US. 

Each line corresponds to the category list of one place, where the list consists of a number of category instances
(e.g., hotels, restaurants, etc.) that are separated by semicolons.

An example line is provided below:
 Local Services;IT Services & Computer Repair

In the example above, the corresponding place has two category instances: "Local Services" and "IT Services & Computer Repair".


## Output
You need to implement the Apriori algorithm and use it to mine category sets that are frequent in the input data.

After implementing the Apriori algorithm, please set the relative minimum support to 0.01 and run it on the 77,185 category lists.
In other words, you need to extract all the category sets that have an absolute support larger than 771.


write all the frequent category sets along with their absolute supports into a text file named "patterns.txt".
Every line corresponds to exactly one frequent category set and should be in the following format:

support:category_1;category_2;category_3;...

For example, suppose a category set (Fast Food; Restaurants) has an absolute support 2851, then the line corresponding to this frequent category set in "patterns.txt" should be:

2851:Fast Food;Restaurants


## Important Tips
format each line correctly in the output file. 
use a semicolon instead of another character to separate the categories for each frequent category set.

In the result pattern file, the order of the categories does not matter.
For example, the following two cases will be considered equivalent.

 Case 1:
 2851:Fast Food;Restaurants

 Case 2:
 2851:Restaurants;Fast Food

---------------------
# Implementation flow 

 1. get the text file and reshape for data frame 
 2. use appriori algorithm and get frequent pattern
 3. save in csv(or text ) file 
