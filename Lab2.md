# CSE15L Lab Report 2
![Image](CSE15L_Lab2_SC1.jpg)


## Part 1
![Image](CSE15L_Lab2_SC2.jpg)
1. The handleRequest method of the Handler class was called. Within the handleRequest method, the getPath() method was called to get the path portion of the uri as a string, .equals()
was called to compare the value of the hard coded string "add-message" to the string value representing the path of the uri, .split() was called to separate the strings based on a specific 
character and to place those string fragments into an array, and .getQuery() method was called to get the query parameters of the uri. The String.format() method was called to return 
a string that incorporates string values from an array. 
2. Relevant arguments to the handleRequest method is a URI. The .getPath() and .getQuery() method doesn't take any arguments and instead, it's a built in URI datatype method that acts on the uri object. 
The .equals() method takes in a string argument that is used to compare with the string formatted output of .getPath(). The .split() method takes in a string argument that represents the substring
used to split the string with. The substring's index is the exact location of the split and the split method's array output omits the substring. The String.format() method's relevant arguments
include a string literal that outlines how variable and non-string-literal values can be nested into the string for output.
3. With this request, the uri that is passed in to our handleRequest function is specific to the uri that was typed typed into the browser. In our uri, we specified the path "/add-message" which allows the if statement condition to evaluate to true. The variable parameters is a string array that holds `{"s=what\'s up brother", "user=Jackie"}` after the url is passed in. value1 and value2 variables are both string arrays that hold two string elements each, where each pair represents the result of splitting the string representing the parameters at the equal sign. This means that value1 holds `{"s", "what\'s up brother"}` and value2 holds `{"user", "Jackie"}`. The element at index position 1 of both value1 and value2 string arrays are then passed to String.format, which uses variables references `%s` (denotes that variable is of string data type), to embed the string values held at index 1 of each string array. 

![Screenshot add-message trial 2](CSE15L_Lab2_SC3.jpg)
1. The handleRequest method of the Handler class was called. Within the handleRequest method, the getPath() method was called to get the path portion of the uri as a string, .equals()
was called to compare the value of the hard coded string "add-message" to the string value representing the path of the uri, .split() was called to separate the strings based on a specific 
character and to place those string fragments into an array, and .getQuery() method was called to get the query parameters of the uri. The String.format() method was called to return 
a string that incorporates string values from an array.
2. Relevant arguments to the handleRequest method is a URI. The .getPath() and .getQuery() method doesn't take any arguments and instead, it's a built in URI datatype method. 
The .equals() method takes in a string argument that is used to compare with the string formatted output of .getPath(). The .split() method takes in a string argument that represents the substring
used to split the string with. The substring's index is the exact location of the split and the split method's array output omits the substring. The String.format() method's relevant arguments
include a string literal that outlines how variable and non-string-literal values can be nested into the string for output.
3. With this request, the url that is passed into our handleRequest function, compared to the above example, is different. In our uri, we specified the path "/add-message" which allows the if statement condition to evaluate to true. The variable parameters is a string array that holds `{"s=slay sister", "user=Esme"}` after the url is passed in. value1 and value2 variables are both string arrays that hold two string elements each, where each pair represents the result of splitting the string representing the parameters at the equal sign. This means that value1 holds `{"s", "slay sister"}` and value2 holds `{"user", "Esme"}`. The element at index position 1 of both value1 and value2 string arrays are then passed to String.format, which uses variables references `%s` (denotes that variable is of string data type), to embed the string values held at index 1 of each string array. 

## Part 2
![Image](CSE15L_Lab2_SC4.jpg)

## Part 3
I learned in week 2 how url requests are parsed and handled by servers and how SSH keys is used to authorize users for secure communication between servers.
I've never understood how private and public SSH keys work together and have always thought of SSH keys as a general password-like authorization. 
