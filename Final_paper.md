# ML final paper

Normal prediction would just give out a price, but we didn't consider uncertainty (whether customer accept or not)

## 2 Data description
## 3 Methodology
3.1 problem formulation
We have ... observational data samples {xi, pi, yi}, where x are features of customers, pi is the price assigned to them, and yi is whether they bought the insurance or not. 
rescriptive trees are trained on observational data, and require three distinct types of data:

Prescriptive trees are trained on observational data, and require three distinct types of data:

X: the features for each observation that can be used as the splits in the tree - this can be a matrix or a dataframe as for classification or regression problems
treatments: the treatment applied to each observation - this is a vector of the treatment labels similar to the target in a classification problem
outcomes: the outcome for each observation under the applied treatment - this is a vector of numeric values similar to the target in a regression problem

treatments: the treatment applied to each observation - this is a vector of the treatment labels similar to the target in a classification problem
outcomes: the outcome for each observation under the applied treatment - this is a vector of numeric values similar to the target in a regression problem
https://docs.interpretable.ai/stable/OptimalTrees/quickstart/prescription/#Data-for-prescriptive-problems

Controls grid search over parameter combinations in param_grid to find the best combination of parameters for lnr.

lnr is a learner with any parameters that should be included in all combinations of parameters tested.

param_grid contains the parameter ranges to search over. These can be supplied in multiple ways, which we demonstrate with examples that create identical GridSearchs to tune lnr over the parameters criterion and normalize_X:


3.2 data preprocess
- convert Vehicle_Age to 0/1/2
- Vehicle_Damage yes/no to 1/0
- Region_Code ()/Policy_Sales_Channel keep 5 categories and others 

price discretization

