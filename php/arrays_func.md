### Arrays and Functions 

Sometimes you'll want to store more than one value within your variables. With an array, you can do just that! Arrays allow you to store multiple values within a variable.
<br>
```php
$cars1 = "Volvo";
$cars2 = "BMW";
$cars3 = "Toyota";
```
But, I'd like to keep things neat n' tidy and have all my cars in a single variable. So I'll use an array, like so:
```php
	$cars = array("Volvo", "BMW", "Toyota");
```
Each value is automatically assigned a "key" in the array, so we can grab a specific value when we need it. We'll touch on keys later, but by default, each value has a numeric key assigned to it.

So for example, __Volvo__ is 1, __BMW__ is 2, and __Toyota__ is 3. Here's the catch though — the numbers start at 0, not 1. So, __Volvo__ is actually 0, etc.

If we want to grab a value out of an array and display it on our web page, we just reference the array and the key associated with the value we want to display, like so:

```php
	echo $cars1[0]; // this will display "Volvo"
	echo $cars2[1]; // this will display "BMW"
 	echo $cars3[2]; // this will display "Toyota"
```
### Associative Arrays
<br>
Remember how PHP automatically assigns a number to each item in an array? Well, using Associative Arrays you can give a custom name to the key, rather than using a number. It looks like this:

```php
	$handlebar = array(
				
		"name" => "Handlebar",				
		"creep_factor" => "High",
		"avg_growth_days" => 14
				
	);
```
			
Now, let's say I wanted to display specific information from the array. I would do so by simply referring to a custom key in the array, like this:

```php
<?php echo $handlebar["creep_factor"]; ?>
```

### Multi-Dimensional Arrays

This is where we start getting crazy! We can harness the true potential of arrays by using multi-dimensional arrays — which is simply an array that is comprised of multiple arrays!

```php
	$moustaches = array (

			array (
			"name"				=> "Handlebar",
			"creep_factor"		=> "High",
			"avg_growth_days"	=> 14
					
			),
					
			array (			
			"name"				=> "Salvador Dali",
			"creep_factor"		=> "Extreme",
			"avg_growth_days"	=> 62
					
			),
					
			array (		
			"name"				=> "Fu Manchu",
			"creep_factor"		=> "Very High",
			"avg_growth_days"	=> 58
					
			)

	);
```
You're probably wondering how the heck we display this info on the screen! Well, we first have to reference the parent array $moustaches, then the numerical value of the child array (Handlebar is [0], Salvador Dali [1], etc), and finally the custom key of the information we want to display (name, creep_factor, etc). It looks like this:

```php 
	<?php echo $moustaches[2]["name"]; ?>
```
The above code will display __Fu Manchu__.

### Funtions
- Built-in Functions
- User Defined Functions










