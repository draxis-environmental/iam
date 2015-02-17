# IAM

Proof of concept time/task tracking UI.

## Idea

There are currently three things each entry is interested in and that can auto complete.

 * **#**project  
   Project currently working on. `#proj-1`, `#proj-2`, etc
 * **@**username  
   Friend or foe you wanna tag. `@geoah`, `@stek`, etc
 * **+**time  
   How long has it been since? `+1h15m`, `+45min`, etc

## Development

Development requires `nodejs >= v0.10.0` with a couple of globally installed packages.  
A simple `npm install -g yo angular-generator grunt-cli bower` should set everything up for you.

Running `grunt serve` will start a web server accessible on `http://localhost:9000`.  
That should be enough for now as nothing else really works.

## Building

To make the application into an executable you will need to build it and package it.  
Building the application using `grunt build` will create a `./dist` folder with
everything you need.  
After that running `grunt nodewebkit` will take the built and package it nicely
into windows and osx applications inside the `./builds` folder.  
*The first time this might take a while as it will need to download the `nw.js` binaries.*
