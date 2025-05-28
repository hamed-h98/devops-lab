# JSON (JavaScript Object Notation)

It's a data representation format similar to xml or yaml

Commonly used for APIs and config files and things like games in text editors like VSCode. 

Lightweight and easy to read/write ccompared to something like xml, since it's much cleaner. 

It's integrated very nicely with javascript since JSON is superset of javascript. 

Anything we write in JSON is valid javascript. so it can be used for front-end or backend of web applications. 

It integrates easily with most languages. 

Every major language has some form of library or built-in functionality to parse json strings into objects or classes in that language. 

So working with json data is very easy inside of a programming language. 

For creating an API, consuming an API, or creating config files for ourself or others to use our application, we use json. 

---

### JSON Types

- Strings: "Hello World" "I"

- Numbers: 10, 1.5, -30, 1.2e10

- Booleans: true, false 

- Null

- Arrays: [1,2,3], ["Hello", "World"]

- Objects: {"key" : "value"} {"age":30}


The objects has pair of key and its value. 

---

### How to use json inside of a file: 

we create a file with `.json` extension 

we use {} for openning and clossing objects 

```json
{
"key" : "value",
"age" : 30,
"name" : "Kyle",
"isCool" : true,
"hobbies" : ["weight Lifting", "Bowling"],

"friends" : [{
    "name" : "Joey",
    "favoriteNumber" : 100,
    "isProgrammer" : true,
    "friends" : []
}]

}
```

---

```json
[
    {
        "Name" : "Big Corporation",
        "NumberOfEmployees" : 1000,
        "ceo" : "Steve",
        "rating" : 3.6
    },
    {
        "name" : "small Startup",
        "numberOfEmployees" : 3, 
        "ceo" : null,
        "rating" : 4.2
    }
]
```

Then we can open `html` file and put javascript in it to run our web page:

```html
<!DOCTYPE html>
<html>
<head>
    <title>JSON Example</title>
</head>
<body>
    <script type = "text/javascript">
        let companies = 
        [
            {
                "Name" : "Big Corporation",
                "NumberOfEmployees" : 1000,
                "ceo" : "Steve",
                "rating" : 3.6
            },
            {
                "name" : "small Startup",
                "numberOfEmployees" : 3, 
                "ceo" : null,
                "rating" : 4.2
            }
        ]
    console.log(JSON.parse(companies))
    </script>
</body>
</html>
```



