# daily-javascript-q18

You have the following HTML page and its referenced Common6.js file: 
```html
<!DOCTYPE html> 
<html> 
<head> 
      <title>Intro to JavaScript</title> 
          	<meta charset="utf-8" /> 
      <script src="Scripts/Common6.js"></script> 
</head> 
<body> 
      <div id="result"></div> 
      <script> 
           function doAction(data, size) { 
                if (!data || size <= 0) 
                     return -1; 
                var newData = data.split(' '); 
                var result; 
                for (var i = 0; i < size; i++) { 
                     result += newData[i]; 
                } 
                return result; 
           } 
      </script> 

      <script> 
           var info = "1 2 3 4 5 6 7" 
           document.getElementById("result").innerHTML = doAction(info, 5); 
      </script> 
</body> 
</html> 
```
Common.js 
```javascript
function doAction(data) { 
      if (!data) 
           return -1; 
      var newData = data.split(' '); 
      var result = 0; 
      for (var i = 0; i < 5; i++) { 
           result += newData[i]; 
      } 
      return result; 
} 
```
What will be displayed in the browser when previewing the page?

Choose the correct answer

1) 012345
2) 15
3) 12345
4) undefined12345
