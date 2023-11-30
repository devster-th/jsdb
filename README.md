# jsdb
A very simple json database for node.js. Has 2 modes, secure and plain. The secure mode encrypts the data so people can't see the data inside.

# dependencies
it needs the `xfile.js and xcrypto.js`, put these files into the `jsdb.js` you're running.

# use
    //in your main program
    const {jsdb} = require('./jsdb')

    //find all in db
    let result = await jdsb.r()

    //find from 'people' collection
    let result = await jsdb.r('people',{name:'john'})

    //write data
    jsdb.w('people',{name:'jane', age:19, sex:'female'})  
    //each adding doc will have the field _id & _time automatically


# files
files you need to run:  
    `jsdb.js, xfile.js, xcrypto.js` ...can find from http://github.com/devster-th

the db file is:  
    `jsdb.json`         //for plain mode  
    `jsdb.sec`         //for secured mode this is base64 encrypted data  
    `jsdb-doc.html`    //this will be a doc file 


# license
none
