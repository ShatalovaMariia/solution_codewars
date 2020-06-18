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
```