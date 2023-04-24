[1.Square Every Digit](https://edabit.com/challenge/BFnsRqe8PFvEwcRNt)

Solution 

```js
function makePair(num) {
     return parseInt(String(num).split('').map( x => Math.pow(x, 2)).join().replace(/,/g,''))
}
```

[2.Mirror Array](https://edabit.com/challenge/BFnsRqe8PFvEwcRNt)

Solution 

```js
function repit(arr){
let x = [...arr];
let result = x.concat(arr.reverse().slice(1,arr.length))
return result;
}
alert(repit([0, 2, 3, 4]));
```

[3.Narcissistic Number](https://edabit.com/challenge/BFnsRqe8PFvEwcRNt)

Solution 

```js
function repit(arr){
let x = [...arr];
let result = x.concat(arr.reverse().slice(1,arr.length))
return result;
}
alert(repit([0, 2, 3, 4]));
```

[4.ReverseAndNot](https://edabit.com/challenge/BFnsRqe8PFvEwcRNt)

Solution 

```js
function repit(arr){
let x = [...arr];
let result = x.concat(arr.reverse().slice(1,arr.length))
return result;
}
alert(repit([0, 2, 3, 4]));
```

[5. Automorphic Number](https://edabit.com/challenge/BFnsRqe8PFvEwcRNt)

Solution 

```js
function repit(arr){
     let num = Math.pow(arr, 2);
     let strNum = num.toString().endsWith(`${arr}`)
     if (strNum) {
      return true;
     }    
     else{
     return false 
     }
}
alert(repit(3))
```

[6.IsItATriangle](https://edabit.com/challenge/BFnsRqe8PFvEwcRNt)

Solution 

```js
function repit(a, b, c){
if (a+b==c && b+c==a&& a+c==b ){
     return true;
}
else{
     return false;
}
}
```

[7.Return Odd > Even](https://edabit.com/challenge/BFnsRqe8PFvEwcRNt)

Solution 

```js
const func = arr =>{
     let a = 0;
     let b= 0;
     arr.map((val)=>{
     val%2==0? a+=1:b+=1
     })
     return a>b;
}
```

[8.Rotate for Max Number]()

Solution

```js
const func2 = num =>{
  return (
    parseFloat(
      num
        .toString()
        //toString making nums to string
        .split('')
        //split() making string to array ["1", "2", "3"]
        .reverse()
        //reverse our array ["3", "2", "1"]
        .join('')
        // join("") all our elems in arr to one string 
    ) * Math.sign(num)
  )                 
}
```

[9.Neatly Formatted Math]()

Solution

```js
const func3 = (a, b, c) =>{
    const func3 = (a, b, c) =>{
     let plus = "+"
     let minus = '-'
     let mltpl = '*'
     let devition = '/'
     if (c==plus) { 
      return  `${a+b}` 
     }
     if (c==minus) { 
       return  `${a-b}` 
      }
      if (c===mltpl) { 
       return  `${a*b}` 
      }
      if (c===devition) { 
       return  `${a/b}` 
      }
      else{
        return false
      }
}
}
```

[10.Is the Number Symmetrical?]()

Solution

```js
function reverseNum(num) {
    for (let i = 0; i < num.length / 2; i++) {
        if (num[i] != num[num.length - i - 1]) {
            return false;
        }
    }
    return true;
}
 
console.log(isPalindrome("12345"));
```