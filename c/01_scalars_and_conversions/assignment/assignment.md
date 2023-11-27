# setup
You need a c-compiler (e.g. gcc) on your machine,
as well as a debugger (e.g. gdb).
Read on how to compile a c program and how to execute it in your debugger.

# 1.1
Limits are defined in an include-header called `limits.h`.
You can read about it here: [tutorialspoint](https://www.tutorialspoint.com/c_standard_library/limits_h.htm)

Write a program that defines a local variable of type signed inside your main-function and assigns to it the highest possible value that can be stored inside a signed int.

Increment this value by one. What value do you expect to see?
Is this new value equal to another constant defined in the limits header?

Add a second variable of type unsigned int, and assign the highest int value possible to it. Increment it by 1 and compare the result to the int case.

# 1.2
Assign 3.14 to a local variable of type float in your main-function.
Add a second variable of type int, and assign the value of your float-variable to it. What value do you expect?

# 1.3
Write a function `round` that takes a float as an argument,
and returns an int, and rounds the value up if its decimal part
is .5 or higher and rounds it down if it's less than .5.

# 1.4
Define an enum `WeekDay` with the following values:
`MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY, SUNDAY`.
Use `typedef` so that this enum becomes a named type.
Define a local variable of that enum type like so:
```c
WeekDay myWeekDay = SUNDAY;
```
Does this definition work? What does it say about the scope of enum values?

# 1.5
Build upon your previous program.
Write a function `nextDay` that takes as argument a `WeekDay`, 
and returns the next day. Note that after sunday should come monday.