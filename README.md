# MongoDB $inc Operator on String Field

This repository demonstrates an example of an uncommon error in MongoDB: using the `$inc` operator on a string field.

The `$inc` operator is designed to increment a numerical value. Applying it to a string field will result in unexpected behavior.  This example showcases the problem and provides a solution.

## Bug
The `bug.js` file contains code that attempts to increment a string field using the `$inc` operator.  This will likely throw an error or produce unexpected results.

## Solution
The `bugSolution.js` file shows the correct approach: either converting the string field to a number before incrementing or using a different operator altogether, such as `$set`, for string manipulation. 