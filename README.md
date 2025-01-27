# MongoDB Aggregation: Incorrect $inc Usage

This repository demonstrates a common error encountered when using the `$inc` operator within MongoDB's aggregation framework. The `$inc` operator is designed for updating documents, not for performing arithmetic operations during aggregation.

The example shows an attempt to increment the 'count' field using `$inc` within the `$project` stage. This approach is incorrect and will likely result in unexpected behavior or errors.

The solution demonstrates the correct way to increment the count by using the `$add` operator instead.

## Bug

The `bug.js` file contains the incorrect implementation.  The `$inc` operator is used improperly leading to incorrect aggregation results.

## Solution

The `bugSolution.js` file provides the corrected implementation, utilizing the `$add` operator to achieve the desired result.