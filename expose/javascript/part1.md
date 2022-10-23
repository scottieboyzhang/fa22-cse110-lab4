# Answer for Part1

## Question 1: 
values added:  20
## Question 2:
final result:  20

```
zhangyuqin@MacBook-Pro fa22-cse110-lab4 % node part1-question1.js 
values added:  20
final result:  20
```

## Question 3:
values added:  20

## Question 4:
ReferenceError: result is not defined
This is because let defines the variable in the if scope, while line 13 is out of the 
scope of if statement.
```
zhangyuqin@MacBook-Pro fa22-cse110-lab4 % node part1-question1.js
values added:  20
/Users/zhangyuqin/fa22-cse110-lab4/part1-question1.js:13
    console.log('final result: ',result);
                                 ^

ReferenceError: result is not defined
    at sumValues (/Users/zhangyuqin/fa22-cse110-lab4/part1-question1.js:13:34)
    at Object.<anonymous> (/Users/zhangyuqin/fa22-cse110-lab4/part1-question1.js:16:1)
    at Module._compile (node:internal/modules/cjs/loader:1159:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1213:10)
    at Module.load (node:internal/modules/cjs/loader:1037:32)
    at Module._load (node:internal/modules/cjs/loader:878:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:82:12)
    at node:internal/main/run_main_module:23:47
```

## Question 5&6:
The code has an error because it is trying to modify a const variable which is illegal.

```
zhangyuqin@MacBook-Pro fa22-cse110-lab4 % node part1-question1.js
/Users/zhangyuqin/fa22-cse110-lab4/part1-question1.js:7
        result = num1 + num2;
               ^

TypeError: Assignment to constant variable.
    at sumValues (/Users/zhangyuqin/fa22-cse110-lab4/part1-question1.js:7:16)
    at Object.<anonymous> (/Users/zhangyuqin/fa22-cse110-lab4/part1-question1.js:16:1)
    at Module._compile (node:internal/modules/cjs/loader:1159:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1213:10)
    at Module.load (node:internal/modules/cjs/loader:1037:32)
    at Module._load (node:internal/modules/cjs/loader:878:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:82:12)
    at node:internal/main/run_main_module:23:47
```

# Answer for Part2

## Question 1:
The output is 3. Since var is declared as function scope, the variable i will be incremented three times due the size of the array is three. Thus, i will store the value of 3.
```
zhangyuqin@MacBook-Pro javascript % node part2-question1.js
3
```
## Question 2:
The output is 150. discountedPrice will store the last value of itself, which will be calculated as 300 * (1 - 0.5) which is 150.
```
zhangyuqin@MacBook-Pro javascript % node part2-question1.js
150
```
## Question 3:
The output is 150. It is because at line8, where the rounding value of discountedPrice is assigned to finalPrice which is 150.
```
zhangyuqin@MacBook-Pro javascript % node part2-question1.js
150
```
## Question 4:
It will return a stack where stores the price of given items after discounts.
In the for loop, firstly we calculated the discountedPrice and then round it. At last we push the modified value to the discounted.
## Question 5:
It has an error because we are using let to declare varible which means the variable is only defined in the block, where in this case, it is the for loop.
```
/Users/zhangyuqin/fa22-cse110-lab4/expose/javascript/part2-question4.js:12
    console.log(i);
                ^

ReferenceError: i is not defined
    at discountPrices (/Users/zhangyuqin/fa22-cse110-lab4/expose/javascript/part2-question4.js:12:17)
    at Object.<anonymous> (/Users/zhangyuqin/fa22-cse110-lab4/expose/javascript/part2-question4.js:19:1)
    at Module._compile (node:internal/modules/cjs/loader:1159:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1213:10)
    at Module.load (node:internal/modules/cjs/loader:1037:32)
    at Module._load (node:internal/modules/cjs/loader:878:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:82:12)
    at node:internal/main/run_main_module:23:47
```
## Question 6:
It is the same reason as the question 5. Since discountedPrice is defined by using let, it is only defined in the scope of for block.
```
zhangyuqin@MacBook-Pro javascript % node part2-question4.js
/Users/zhangyuqin/fa22-cse110-lab4/expose/javascript/part2-question4.js:12
    console.log(discountedPrice);
                ^

ReferenceError: discountedPrice is not defined
    at discountPrices (/Users/zhangyuqin/fa22-cse110-lab4/expose/javascript/part2-question4.js:12:17)
    at Object.<anonymous> (/Users/zhangyuqin/fa22-cse110-lab4/expose/javascript/part2-question4.js:19:1)
    at Module._compile (node:internal/modules/cjs/loader:1159:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1213:10)
    at Module.load (node:internal/modules/cjs/loader:1037:32)
    at Module._load (node:internal/modules/cjs/loader:878:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:82:12)
    at node:internal/main/run_main_module:23:47

Node.js v19.0.0
```
## Question 7:
The output is 150. Since finalPrice is defined by let but in the function scope. Thus, it stores the value of the final price the last item, which is 150.
```
zhangyuqin@MacBook-Pro javascript % node part2-question4.js
150
```
## Question 8:
It will return a stack where stores the price of given items after discounts.
In the for loop, firstly we calculated the discountedPrice and then round it. At last we push the modified value to the discounted. Even if it is defined by let, it is in the scope of the funtion.
## Question 9:
It has an error because we are using let to declare varible which means the variable is only defined in the block, where in this case, it is the for loop.
```
zhangyuqin@MacBook-Pro javascript % node part2-question9.js
/Users/zhangyuqin/fa22-cse110-lab4/expose/javascript/part2-question9.js:10
    console.log(i);
                ^

ReferenceError: i is not defined
    at discountPrices (/Users/zhangyuqin/fa22-cse110-lab4/expose/javascript/part2-question9.js:10:17)
    at Object.<anonymous> (/Users/zhangyuqin/fa22-cse110-lab4/expose/javascript/part2-question9.js:16:1)
    at Module._compile (node:internal/modules/cjs/loader:1159:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1213:10)
    at Module.load (node:internal/modules/cjs/loader:1037:32)
    at Module._load (node:internal/modules/cjs/loader:878:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:82:12)
    at node:internal/main/run_main_module:23:47
```
## Question 10:
The output is 3. Length is defined by const which stores the length of the given array which is 3.
```
zhangyuqin@MacBook-Pro javascript % node part2-question9.js
3
```
## Question 11:
It will return an empty array. Since discounted is defined as const, it cannot be modified. The push command will not do anything to the array. Thus, the array is still empty.


