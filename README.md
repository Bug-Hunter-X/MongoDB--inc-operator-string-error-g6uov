# MongoDB $inc operator string error
This example demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numerical field by a specified value. However, if a string is provided as the increment value, the operation will fail to increment the field correctly.

**Bug:**
The bug lies in providing a string '1' instead of a number 1 as the increment value in `$inc: { field: '1' }`. This results in an incorrect update, where the field might not be incremented as expected or an error might occur.

**Solution:**
Ensure the increment value provided to the `$inc` operator is a number, not a string.
