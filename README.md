# issue
Had fetched risk type data for a certain timestamp & match it with cobble epochs of similar timestamp in a target column with [1,0]. Using available dataset need to built a confusion matrix, so that will get an idea about False positives and True negatives among them. I wanted to know what approach should taken for splitting of feature variables and target variables for plotting.
Have 2 methods discussed now:

    Like usual train_test_split by dividing dataset as xtrain ,xtest, ytrain, ytest with 'target' column as 'y' and remaining columns as 'x'.
    Calculate sum of all risk values for each timestamp into one column,normalize them,by providing a threshold (like > 0.5=1 and < 0.5=0) split them o a new column of 1's and 0's and find confusion matrix with respect actual 'target' column and new 'predicted' column.
