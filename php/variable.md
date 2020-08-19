### Variables and Data Types

>>Think of a variable as a bucket. Literally, a bucket. That bucket can hold stuff in it — like food, or dirt. In PHP, variables are buckets, but instead of holding food or dirt, they hold information — like numbers, text, images, or logic! All you need to know at this point is that variables are buckets that store information for later use. We'll get to how we actually use the variables in an upcoming lecture. <br>
<br>
>>The basic syntax of a variable is a dollar sign ($) directly followed by a variable name (using text, with no spaces), then an equal sign, followed by the contents of the variable, ending with a semi-colon. <br>

```php
	$variable_name = 'my first variable';
```
There are 4 basic variable types, and each type of variable (or "bucket") is meant to hold specific information. <br>

+ Boolean
A boolean variable specifies a value of true or false. <br>

```php
    $logged_in = true;
```
+ Integer
An integer variable is any whole number. <br>

```php
    $fav_num = 2940;
```
+ Floating Point
Usually a fractional number, with a decimal. <br>

```php
    $top_speed = 104.87;
```

+ String
Simple text that must be enclosed within double quotations " " or single quotations ' ' <br>

```php
    $vehicle = "Subaru";
```

#### Here are some more basic variables:
```php
    $my_name = "deep";
     
    $my_age = 23;
     
    $fav_colour = "Black";
```
If I want to display these variables on the page in some meaningful way, I could use the PHP Print Function: <br>

```php
	print("My name is $my_name! <br>
	I'm $my_age years old, and like the colour $fav_colour.");
```
### Defining Constants

A constant is similar to a variable in the sense that you can store information in a keyword that can be used throughout your web page. However, the value of a constant cannot be changed, unlike a variable. It's literally "constant". <br>

It's also worth noting that constants are case-sensitive and are written in ALL CAPS by convention. Here's how you define a constant in PHP:

```php
define("TITLE", "Defining Constants");
To display a constant on your page, you can echo it using PHP, like this:
```

```php
	<?php echo TITLE; ?>	
```

Back to [Documentation](https://github.com/dkhatri481/learnCode)
