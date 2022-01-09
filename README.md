# SNOW-JavaScript-JSON

What is JSON?

- JSON stands for JavaScript Object Notation
- JSON is a lightweight data-interchange format
- JSON is "self-describing" and easy to understand
- JSON is language independent *

## JSON is a syntax for storing and exchanging data.
- JSON is text, written with JavaScript object notation.
- When exchanging data between a browser and a server, the data can only be text.
- JSON is text, and we can convert any JavaScript object into JSON, and send JSON to the server.
- We can also convert any JSON received from the server into JavaScript objects.
- This way we can work with the data as JavaScript objects, with no complicated parsing and translations.


## JSON syntax is derived from JavaScript object notation syntax:
- JSON data is written as name/value pairs.
- Data is separated by commas
- Curly braces hold objects
- Square brackets hold arrays
- A name/value pair consists of a field name (in double quotes), followed by a colon, followed by a value:
- Eg :
         "name":"John"

## JSON.parse()
JSON is used to exchange data to/from a web server.
When receiving data from a web server, the data is always a string.
Parse the data with JSON.parse(), and the data becomes a JavaScript object.
```
<!DOCTYPE html>
<html>
<body>

<h2>Create Object from JSON String</h2>

<p id="demo"></p>

<script>
var txt = '{"name":"John", "age":30, "city":"New York"}'
var obj = JSON.parse(txt);
document.getElementById("demo").innerHTML = obj.name + ", " + obj.age;
</script>

</body>
</html>

```

## JSON.stringify()
- JSON is used to exchange data to/from a web server.
- When sending data to a web server, the data has to be a string.
- Convert a JavaScript object into a string with JSON.stringify().

```
<!DOCTYPE html>
<html>
<body>

<h2>Create JSON string from a JavaScript object.</h2>

<p id="demo"></p>

<script>
var obj = { name: "John", age: 30, city: "New York" };
var myJSON = JSON.stringify(obj);
document.getElementById("demo").innerHTML = myJSON;
</script>

</body>
</html>
```

JSON vs JS object
![image](https://user-images.githubusercontent.com/12488769/148701587-7c23ed0d-79d2-457e-a854-2b8c82fafb11.png)



