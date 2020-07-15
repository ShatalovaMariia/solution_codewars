# Localize The Barycenter of a Triangle
```javascript
function barTriang(p1, p2, p3){
    let p0 = +((p1[0] + p2[0] + p3[0])/3).toFixed(4);
    let p4 = +((p1[1] + p2[1] + p3[1])/3).toFixed(4);
    return [p0, p4];
}
```
# Calculate Price Excluding VAT
```javascript
function excludingVatPrice(price){
 
  return (price === null)? -1 : +((price / 115)* 100).toFixed(2);
}
```
# How many stairs will Suzuki climb in 20 years?
```javascript
return s.reduce((acc,curr) => acc.concat(curr)).reduce((acc,curr) => acc + curr)* 20; 
}
```
# Parse float
```javascript
function parseF(s) {
let res = Number.parseFloat(s);
console.log(res)
return isNaN(res)? null : res;
}
```
# Find Duplicates
```javascript
function duplicates(arr) {
  return arr.filter((el,i) => arr.indexOf(el) === i && arr.lastIndexOf(el) !== i)
}
```
# Array element parity
```javascript
function solve(arr){
  return arr.find(el => !arr.includes(-el))
}
```
# Sum of Odd Cubed Numbers
```javascript
function cubeOdd(arr) {
let sum = 0;
for( let i = 0;i < arr.length;i++){
if (arr[i] % 2 !== 0) 
sum = sum + arr[i] ** 3;
if(typeof arr[i] !== 'number') return undefined;
}
return sum;
}
```
# Divide and Conquer
```javascript
function divCon(x){
let sum1 = 0;
let sum2 = 0;
for(let i = 0;i < x.length;i++){
 if(typeof x[i] === 'string') 
 sum1 = sum1 + +(x[i]);
 console.log(sum1);
 if(typeof x[i] === 'number')
 sum2 = sum2 + x[i];
}
return sum2 - sum1;
}
```
# Count by X
```javascript
function countBy(x, n) {
  var z = [];
for(let i = 1;i <= n ;i++){
  
  z.push(i * x)
  }
  return z;
}
```
#Generate range of integers
```javascript
function generateRange(min, max, step){
let arr = [];
  for(let i = min;i <= max;i = i+step){
    arr.push(i)
}
return arr;
}
```
# Powers of 2
```javascript
function powersOfTwo(n){
  let arr = [];
  for(let i = 0; i <= n;i++){
    arr.push(2 ** i)
  
}
return arr;
}
```
# Be Concise IV - Index of an element in an array
```javascript
let find=(arr, el)=> {
  let a = arr.indexOf(el)
  return (a != -1)? a: "Not found";
}
```
# The Office IV - Find a Meeting Room
```javascript
function meeting(x){
 for(let i = 0;i < x.length;i++){
   if (x[i] === 'O') return x.indexOf(x[i])
 }
   return 'None available!'
}
```

# No Loops 2 - You only need one
```javascript
function check(a,x){
  if (a.includes(x))
  return true
  else return false
};
```
# Train to remove duplicates from an array with filter()
```javascript
function unique(arr) {
return arr.filter((el,i )=>  i === arr.indexOf(el));

}
```
#Two to One
```javascript
function longest(s1, s2) {
 let res = (s1 + s2).split('').sort();

 let res2 = res.filter((el,i) => res.indexOf(el) === i);
 return res2.join('');

}
```
# Array element parity
```javascript
function solve(arr){
  return arr.find(el => !arr.includes(-el))
};
```
# Convert number to reversed array of digits
```javascript
function digitize(n) {
 let str = n + '';
  return str.split('').reverse().map(el => +el)
}
```