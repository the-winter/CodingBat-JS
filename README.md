# CodingBat-JS

Click on the Array-1.ipynb file to find answers.

The answers are written along with their questions, like this:

```js
// array-1
// firstLast6
/**
Given an array of ints, return true if 6 appears as 
either the first or last element in the array. 
The array will be length 1 or more.
**/

function firstLast6(nums) {
  if (nums[0]==6) {return true}
  else if (nums[nums.length-1]==6) {return true}
  else {return false}
}
```

You can ignore this code:

```js
// var assert = require('chai').assert
var _ = require('lodash')
Out[4]:
'use strict'
In [2]:
/** test function to give feedback **/
function t(func,inputs,outputs){
    // this uses the "spread" operator http://es6-features.org/#SpreadOperator
    // TODO: if (func(...inputs)_.isEqual(inputs)){
    
    // runs the  function wih the inputs
    let res = func(...inputs)
    // does the results match the exected outputs?
    let match = _.isEqual(res,outputs)
    // print the results
    if (match){
        console.log(`✔ ${func.name}(${inputs}) == ${outputs}`)
    } else {
        // this uses es6 template literals http://es6-features.org/#StringInterpolation
        console.error(`✖ ${func.name}(${inputs}) != ${outputs}`)
    }
}
```

It is just code I used to test my answers. Likewise, code that looks like this:

```js
t(firstLast6,[[1, 2, 6]],true)
t(firstLast6,[[6, 1, 2, 3]],true)
t(firstLast6,[[13, 6, 1, 2, 3]],false)
t(firstLast6,[[13, 6, 1, 2, 6]],true)
t(firstLast6,[[3, 2, 1]],false)
t(firstLast6,[[3, 6, 1]],false)
t(firstLast6,[[3, 6]],true)
t(firstLast6,[[6]],true)
t(firstLast6,[[3]],false)
t(firstLast6,[[5, 6]],true)
t(firstLast6,[[5, 5]],false)
t(firstLast6,[[1, 2, 3, 4, 6]],true)
t(firstLast6,[[1, 2, 3, 4]],false)
```

is just testing the answers.
