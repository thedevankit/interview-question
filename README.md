# Interview-question

```javascript
// Online Javascript Editor for free
// Write, Edit and Run your Javascript code using JS Online Compiler
    
var arrayOfValues = [1,2,1,2,3,6,4,1,3,8,9,7,3,4,5,7,6,4,2,1,3,0];

//Get Unique values from array
// Method 1 Using set() function
var uniqueArray = [...new Set(arrayOfValues)];

console.log("Unique Array values");
console.log(uniqueArray);

//Unique array sorted 
var sortedArray = uniqueArray.sort();

console.log("Unique sorted array values");
console.log(sortedArray);

secondLargestValue = sortedArray[1];
//Get 2nd smallest and send largest number 
console.log("smallest and send largest number in array");
console.log(secondLargestValue,'2nd Smallest element in array ');
console.log(sortedArray[sortedArray.length-2],'2nd largest element in array ');

console.log(sortedArray);
//Odd and even numbers in array.
oddValues = sortedArray.filter((item)=>item % 2==1);
console.log("Unique sorted odd values first than even values in array");
console.log(oddValues);
console.log(segregateEvenOddnumber(sortedArray))

function segregateEvenOddnumber(sortedArray){
    let j=-1; 
    let temp;    
    for(i=0;i<sortedArray.length;i++){
        if(sortedArray[i]%2==1){
            j++;
            temp = sortedArray[i];
            sortedArray[i] = sortedArray[j];
            sortedArray[j] = temp;
        }
    }
    return sortedArray;
}

// Output:
// [ 1, 2, 3, 6, 4, 8, 9, 7, 5, 0 ]
// Unique sorted array values
// [ 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 ]
// smallest and send largest number in array
// 1 '2nd Smallest element in array '
// 8 '2nd largest element in array '
// [ 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 ]
// Unique sorted odd values first than even values in array
// [ 1, 3, 5, 7, 9 ]
// [ 1, 3, 5, 7, 9, 2, 6, 0, 8, 4 ]

```
