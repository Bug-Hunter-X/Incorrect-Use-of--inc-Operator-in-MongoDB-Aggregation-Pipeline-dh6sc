# Incorrect Use of $inc Operator in MongoDB Aggregation Pipeline

This repository demonstrates a common error when using the `$inc` operator within a MongoDB aggregation pipeline.  The `$inc` operator is designed for updating documents, not for performing simple arithmetic within the aggregation framework.  This example shows the incorrect usage and the corrected version.

## Bug
The `bug.js` file contains the incorrect usage of `$inc` within the `$project` stage of the aggregation pipeline. This will either lead to unexpected results or an error. 

## Solution
The `bugSolution.js` file provides the corrected aggregation pipeline, utilizing the `$add` operator instead of `$inc` for the desired increment operation. 