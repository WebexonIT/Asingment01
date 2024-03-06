# Asingment01
php work

Differences between $var and $$var in PHP

$var:
The $var notation is the standard way of declaring and accessing variables in PHP. It is used to assign a value to a variable and retrieve the stored value later in the code. For example:

$name = "John";
echo $name; // Output: John

$$var
The $$var notation, also known as variable variables, introduces a dynamic approach to variable names in PHP. It allows you to create variables with names based on the value of another variable. Here’s an example:

$var = "name";
$$var = "John";
echo $name; // Output: John


${'var'} 
Both of the instances above are not deprecated, but placing the dollar sign outside the curly brace is deprecated in PHP 8.2 and later. For example, the following snippet emits a deprecation notice:
$name = 'PHP';
$var = 'name';

echo "Hello ${$var}"; // Hello PHP

2. Discuss the importance of variable scoping in PHP. How does PHP handle variable scope?
Ans: Variables are an important part of any programming language. You can use them to store all kinds of information like integers, floats, strings, arrays, the contents of a file, etc. The data stored in variables can then be manipulated by adding or removing information. Using variables also allows us to create loops and perform some tasks repetitively. You can also define functions that take different variables as arguments and give back new data.

What Is Variable Scope?
Variables are used to store and access or manipulate information later, but you cannot just access their data from any place you like. Some variables might become inaccessible in certain places, depending on the programming language you are using.

In simple terms, the scope of a variable determines its availability in different sections of a program.

Variable Scope in PHP
PHP has an easy-to-understand and beginner-friendly approach to variable scope.

A variable you define somewhere in a PHP file will be visible or available almost everywhere after it is defined. You will also be able to use it within other files added to the program using include() and require().


3.
What is variable interpolation in PHP? Provide an example.
Ans: PHP Variable Interpolation
by Vincy. Last modified on July 1st, 2022.
Variable interpolation is adding variables in between when specifying a string literal. PHP will parse the interpolated variables and replace the variable with its value while processing the string literal.

I PHP, a string literal can be specified in four ways,

Single quoted
Double quoted
Heredoc syntax
Nowdoc syntax
Interpolation: The variable parsing is allowed when the string literal is enclosed with double quotes or with heredocs.
Single quoted string or nowdocs, does not support variable interpolation.

<?php
$name = "PHPPOT";
echo "I am reading $name"; // output: I am reading PHPPOT
echo 'I am reading $name'; // output: I am reading $name
?>

4. Describe the concept of variable variables in PHP. Provide an example to illustrate its usage.
Variables in a program are used to store some values or data that can be used later in a program. The variables are also like containers that store character values, numeric values, memory addresses, and strings. PHP has its own way of declaring and storing variables. 
Data types used by PHP to declare or construct variables:

Integers
Doubles
NULL
Strings
Booleans
Arrays
Objects
Resources

<?php

$num = 20;

// function to demonstrate use of global variable
function global_var()
{
	// we have to use global keyword before 
	// the variable $num to access within 
	// the function
	global $num;
	
	echo "Variable num inside function : $num \n";
}

global_var();

echo "Variable num outside function : $num \n";

?>

5. How do you check if a variable is set and not null in PHP? Explain the significance of this check-in preventing errors.
Ans: 
