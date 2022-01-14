# Optimized Including

## What is the benefit?
Normally, two variables are used to add express to your Nodejs project. These are usually saved as **express** and **app**. 
But by saving as two variables, **you get a longer start-up time and a loss of performance.**

## How to use?
To use, instead of using your code as below,
```js
const express = require('express');
const app = express();
```
to this
```js
const app = require('express')();
```

## Disadvantages of using
If you use it this way, you will not be able to use functions such as internal JSON and urlencoded that come with the express, since express is run instead of being assigned to a variable.
