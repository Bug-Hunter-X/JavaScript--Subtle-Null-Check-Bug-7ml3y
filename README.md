# JavaScript Subtle Null Check Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to null checks.

The `bug.js` file contains the erroneous code. The `bugSolution.js` file offers a corrected version.

The core issue lies in the use of loose equality (`==`) when checking for null values.  This operator performs type coercion, potentially leading to incorrect results when comparing against both `null` and `undefined`.

The solution utilizes strict equality (`===`), avoiding type coercion to guarantee accurate null checks.