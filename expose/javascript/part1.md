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
<hr>

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



