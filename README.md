# Dcksy.js
Simple DuckyScript to Teenst converter, based on https://github.com/Thecakeisgit/Dckuino.js. All credits to Thecakeisgit

If you need to perform mouse emulation then use [d4n5h's Duckuino](https://github.com/d4n5h/Duckuino).

*NOTE: If you are on linux, you might use the Arduino IDE from the website, not from apt, because the apt repo is not up to date.*

# Why Dcksy.js

While using Dckuino.js to generate the code to Teensy I found some litle details that I needed to be changing all the time, so that the code would work so

You can use the entire project in the [Live](https://luisfontes19.github.io/Dcksy.js/ "Dcksy.js Live") version, or reuse <code>dcksy.js</code> for standalone use :

```javascript
// Create the instance
Duck = new Dcksy();

var DuckyScript = "CTRL ALT t\n"
+ "DELAY 1000\n"
+ "STRING gedit\n"
+ "ENTER\n"
+ "DELAY 1000\n"
+ "STRING Hello World !"

var TeensyCode = Duck.toTeensy(DuckyScript);

console.log(TeensyCode);
```