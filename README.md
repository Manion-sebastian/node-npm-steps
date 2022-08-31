### Running npm from scratch.

Step 1 install Node.js
```brew install node```
Step 2 install Npm
```npm install```
Step 3 create a new directory
```mkdir "folder name"```
Step 4 inside the new directory touch the files you require
```cd newFolder -> touch index.js index.html styles.css```
Step 5 npm init and confirm all data.
```npm init```
Step 6 add .gitignore to the folder 
Step 7 in .gitignore write node_modules 
this will keep the thousands of lines of code from being pushed to the repo.
You now have a blank canvas for what you want to do. 
Step 8 npm i any modules you wish to use. and if required require them
``` const module = require('module')```
the module is ready for use

### Running npm from a clone.

Step 1 do the above step 1 and 2
Step 2 fork and clone the repo
```git clone url```
should this repo have dependancies use 
```npm i```
this will install everything you need. 
if no .gitignore make one, and then require the modules youre using. 

### Create your own module. 

Step 1 create a file for your module. it will be a .js
Step 2 either create an inline function
```module.exports.beBasic = () => console.log("That's so fetch!")```
or create it with brackets 
```module.exports = {```
``` this and that```
```}```
or if its a class you can do 
```class Car {```
    ```constructor(color, convertible) {```
        ```this.color = color```
        ```this.convertible = convertible```
        ```this.speed = 0```
    ```}```
    ```accelerate(num) {```
        ```this.speed += num```
```}```
    ```decelerate(num) {```
        ```this.speed -= num```
    ```}```
```}```
and export it with a call tot he class name
```module.exports = Car```
