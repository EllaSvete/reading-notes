# class 8 lecture

table footer:

 ``` Javascript
let numsArr = [
  [1, 2, 3],
  [4, 5, 6],
  [7,8,9],

]

console.table(numsArr);

// 1st iteration - add the first column
// numsArr[0][0] = 1
// numsArr[1][0] = 4
// numsArr[2][0] = 7
//numsArr[j][i]

// 2nd iteration - add the 2nd column
//numsArr[0][1] = 2
//numsArr[1][1] = 5
//numsArr[2][1] = 8
//numsArr[j][i]

// 3rd iteration - add the 3rd column
// numsArr[0][2] = 3
// numsArr[1][2] = 6
// numsArr[2][2] = 9
//numsArr[j][i]


for(let i = 0; i < numsArr.length; i++){ // slow
  let total = 0; // 1 after first iteration
  for(let j = 0; j < numsArr.length; j++){ // fast
    total = total + numsArr[j][i]
    //        0.        1
  }
  console.log(total);
}

for(let i = 0; i < numsArr.length; i++){ // slow
  let total = 0; 
  for(let j = 0; j < numsArr.length; j++){ // fast
    total = total + numsArr[j][i]
    grandTotal += numsArr[j][i]; // where will grand total live in table
  }
  console.log(total);
}