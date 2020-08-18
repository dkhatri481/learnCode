### Variables

>> Case-sensitive <br>
>> Should be meaningful and descriptive <br>
>> Cannot start with a number <br>
>> Cannot contain a space or hyphen (-) <br>
>> Cannot be a reserved word <br>

+ var // var declarations are globally scoped or function scoped while let and const are block scoped. var variables can be updated and re-declared within its scope;

```javascript
	
	var name = 'John';  <-- declare
	console.log(name);

```


+ let // let variables can be updated but not re-declared; 

```javascript

	let age;    <--- declare
	age = 30;   <--- initialize the value
	age = 40;
	
	console.log(age);
```

+ constants // const variables can neither be updated nor re-declared;

```javascript
	
	const pi = 3.14
	console.log(pi);

```
Back to [Documentation](https://github.com/dkhatri481/learnCode)
