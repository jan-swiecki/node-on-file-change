node-on-file-change
===================

fs.watch wrapper that among other things checks SHA1 of the file to prevent multiple callback calls.

Related: http://stackoverflow.com/q/12978924/1637178
 
Usage is the same as in `fs.watch`

    var onFileChange = require("on-file-change");
 
    // same as in fs.watch
    onFileChange("file.txt", function()
    {
        console.log("File changed!");
    });

## Installation

`npm install on-file-change`