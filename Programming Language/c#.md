# Learning C#

- It is a general-purpose language that can be used for different types of applications and web-based services. C# is used for developing software, applications, and video games. C# is also used for creating components and controls3. C# is a versatile and popular language among developers.

# Introduction

- `class` - is basically a container where we can store a bunch of codes. Inside class, we can then write codes for our program and it'll be executed by the codes/isntructions written inside it.
- `method/function` - is another container inside `class` where we want to write the codes for our program to execute.
- `Instructions` - is what we want our computer to execute. For example:

```c#
Console.WriteLine("Hello World");
```
The example above is telling the computer to write a line `Hello World`.

- `Console` - is a little window where we can see the output of our codes. 
- `WriteLine("Hello World")` - is the instruction that we want our computer to do which basically says to `Write a Line` and inside the parenthesis which specifies what line should the computer write which is `Hello World`.
- `;` - semicolon is very important and it should be `ALWAYS` at the end of every line of code.
- `Console.ReadLine();` - is an instruction where it lets you see the console or the little window for a while because the computer closes the window immediately after it executes the instruction for example the `WriteLine`.


# Basic Variables
- is a special container where you can store some information that you want to keep track of and manage.

1.  `string` - is an example of a variable where you can store a text inside it.
2. `int` - is also a variable where you can store integers or whole numbers.

There are `2 methods` of writing these variables. One, which is to declare a value to a variable immediately. Two, which is to just write the Variable and naming it and then giving it a value on the next line.

## First Method
```c#
string kingdomName = "Arcadia";
int populationNum = 1000;
```

## Second Method

```c#
string kingdomName;
kingdomName = "Arcadia";
int populationNum;
populationNum = 1000;
```

--- 
---
You can also change a certain `value` of a variable in the middle of the output/text by writing it in the `middle` and changing the value of that variable. As an example:

```c#
string kingdomName;
kingdomName = "Arcadia";
int populationNum;
populationNum = 1000;

            Console.WriteLine("There was a Kingdom named " + kingdomName);
            Console.WriteLine("With a population of " + populationNum);

            
kingdomName = "Alfheim";
populationNum = 500;

            Console.WriteLine("it was named as that until a new king changed it to " + kingdomName);
            Console.WriteLine("as he reigned, the population decreased into " + populationNum);
            Console.WriteLine("the people are not happy because of the current king.");
```

Thus, the result of the command would be

```
There was a Kingdom named Arcadia
With a population of 1000
it was named as that until a new king changed it to Alfheim
as he reigned, the population decreased into 500
the people are not happy because of the current king.
```

Notice how the name of the `Kingdom` and the `Population` changed.

# Different types of Data

## Plain Text:

1. `string *name of the string = "text";` - a string is where you can write a plain text that can be a whole sentence or a few words.
2. `char *name of the char/character = 'S'` - a character or char is where you can write a text and you are only able to put ONE character inside it for example "a, b , c, d etc.. When you need to put more than one character, then you can use `string`.
   
## Numbers:

1. `int *name of the variable integer = *value or number` - a integer or int is where you can write or store a `whole number`.
2. `double *name of the variable double = *a decimal number` - a `double` variable is a variable where you can write or store a `decimal number` such as "60.3, 12.5, 3.14" as an example.

NOTE: There are 3 types of data types for decimals which are "float - double - decimal" with decimal being used for super accurate uses and float being the least. For now, double would do as a beginner.

## Additional:

- `bool *name of the boolean = *either true or false;` - a boolean is a data type that is a true or false value.

# Working with strings

  1. `\n` - is used to separate words in a string and makes a new line for that.
  
  For example: 
  
  >Console.WriteLine("I am\nAwesome");
```
I am
Awesome
```
  2. `\` - you can use this to write a literal `"` or a `quotation mark` and not turning it into a command or to an error.
  
   For example: 
   
   >Console.WriteLine("I am\"Awesome");

   Result:
```
I am"Awesome
```
 3. `*variable name.Length` - is used to determine how long or how many letters are in a `string`. 

  For example: 
  
  >string title = "I am Vengeance";
  >
  >Console.WriteLine( title.Length );

  Result:
  ```
  14
  ```
  4. `*variable name.ToUpper()` - is used to make the words inside the string be all CAPS. and to have it all on lowercase, just use `ToLower` instead of the former.

 For example:
 >string title = "I am Vengeance";
 >
 >Console.WriteLine( title.ToUpper() );

 Result:
 ```
 I AM VENGEANCE
 ```
 5. `*variable name.Contains()` - is used to identify whether a certain word is inside a string or not.

For Example: 
>string title = "I am Vengeance";
>
>Console.WriteLine( title.Contains("Vengeance") );

Result:
```
True
```
### _**Note**: If the word is not there, then the result would be `False`_.

6. `*variable name[ *index/number order of a character]` - is used to indentify a character in a string.

For Example: 

>string title = "I am Vengeance";
>
>Console.WriteLine( title[5] );

Result:
```
V
```

### _**Note:** Every character starts at `0` not `1`._

7. `*variable name.IndexOf()` - is used to indentify which index position is a word in.

For Example:
>string title = "I am Vengeance";
>
>Console.WriteLine( title.IndexOf("Vengeance") );

Result:
```
5
```
### _**Note:** If you want to indentify a single character, you have to use `'` or a single quotation mark_.

8. `*variable name.Substring()` - is used to grab one single part of a string by writing the index position of the word you want to grab.

For Example:

>string title = "I am Vengeance";
>
>Console.WriteLine( title.Substring(5) );

Result:
```
Vengeance
```
### Another Example:
>Console.WriteLine( title.Substring(5, 3) );

Result:
```
Ven
```
### _The use for that is to grab a part of an word inside a string but only take `3` characters off of it._

# Working with Numbers