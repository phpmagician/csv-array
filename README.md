#CSV-parse

## Dependencies
This package got only one dependency of "fs". You may install that first using following command

```
npm install fs
```

## Usage Guide
After installing the package you can use the "parseCSV" method as follows
```
 parseCSV("CSV-file-name.csv", callBack)
 //where callBack is a function having the argument data 
 //which is an array structure of the CSV file
```
### Example

```javascript
 var csv = require('CSV-parse');
 csv.parseCSV("test.csv", function(data){
   console.log(JSON.stringify(data));
 });
``` 
If the test.csv file contains something like this

```
 Question Statement,Option 1,Option 2,Option 3,Option 4,Option 5,Answer,Deficulty,Category
this is a test question answer it?,answer 1,answer 2,answer3,answer 4,,answer 2,3,test
this is another test question answer it?,"answer1,answer2","answer2,answer3","answer4,answer5","answer5,answer6","answer7,answer8","answer1,answer2",2,test
```

Then the resulting array is as follows
```

```
