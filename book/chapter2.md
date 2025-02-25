# Chapter 2 - Variables
What is a + b?

Well it could be anything. That's because "a" and "b" don't have a value. Let's change that.

```lua
a = 5
b = 3
```

Let's take another look, what is a + b? What we're really asking is "What is the value of a + the value of b?". In other words, what is 5 + 3? Which is 8.

To prove that a + b = 8, we're going to print it. (We're going to use `print` to make the number appear in our output console)

```lua
a = 5
b = 3
print(a + b)
--Output: 8
```

Run your code (meaning press F6 and then close the window to show the output) and your console should say `8` .

`a` and `b` are what we call *variables*. A variable is a word in which you can store a value. The number 4 is always 4, and 35 is always 35, but a variable can be anything you want it to be. Hence the name variable.

The word in which you store a value can be almost anything.
```lua
sheep = 3
test = 20
PANTS = 1040
asdfghjkl = 42
```

Variables are *case-sensitive*. That means that when you have the same word, but with different casing, it's not treated as the same. For example
```lua
sheep = 3
SHEEP = 10
sHeEp = 200
```
are three different variables, with each their own value.

You can do more than just summing up numbers.
```lua
a = 20 - 10 --Substraction
b = 20 * 10 --Multiplication
c = 20 / 10 --Division
d = 20 ^ 10 --Exponentiation
```
For numbers with decimals we use a dot.

```lua
a = 10.4
b = 2.63
c = 0.1
pi = 3.141592
```

Take a look at the following code:

```lua
a = 5
b = 3
c = a + b
```

First we say `a = 5`. When we give a variable a value, we call that an *assignment*. We *assign* 5 to `a`, and 3 to `b`. Next we assign `a + b` to `c`. So now `c` equals 8. Remember that you can always check the value of a variable with `print`. If we were to change the value of `a` or `b` after `c = a + b`, it would not affect `c`. It would still be 8.

```lua
a = 5
b = 3
c = a + b
a = 2
b = 40
print(c)
--Output: 8
```
This is because to the computer `c` is not `a + b`, it's simply 8.

___
## Strings
A variable can also store text.
```lua
text = "Hello World!"
```
This is what we call a *string*. Because it's a string of characters.

We can connect strings by using two dots (..)
```lua
name = "Daniel"
age = "22"
text = "Hello, my name is " .. name .. ", and I'm " .. age .. " years old."
print(text)
--Output: "Hello, my name is Daniel, and I'm 22 years old."
```
___

## Variable naming rules
There are a few rules when naming a variable. First of all, your variable may have a number in it, but not at the start.

```lua
test8 --Good
te8st --Good
8test --Bad, error!
```

Your variable name also can't include any special characters like @#$%^&*.

And finally, your variable name can't be a keyword. A keyword is a word that the programming language uses. Here's a list of keywords:

```nil
and       break     do        else      elseif
end       false     for       function  if
in        local     nil       not       or
repeat    return    then      true      until     while
```

___

## Usage

Variables can be used to keep track of things. For example, we can have to variable `coins`, and every time we pick up a coin we can do `coins = coins + 1`.

___

## Summary
Variables are words in which we can store a value like a number or text. You can name them whatever you want, with a few exceptions. Variables are case-sensitive.