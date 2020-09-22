<div align="center">

## Basics of C/C\+\+ Part 7: Structures


</div>

### Description

Welcome to the seventh lesson. This is my first lesson that I will explain classes. However, I will explain more about structures, because they can be useful, and they are a good way to get a feel for how a class works. What are structures? They are a way to store more than one data-type under the same name.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Alexander of CProgramming\.com](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/alexander-of-cprogramming-com.md)
**Level**          |Intermediate
**User Rating**    |3.8 (23 globes from 6 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/alexander-of-cprogramming-com-basics-of-c-c-part-7-structures__3-459/archive/master.zip)





### Source Code

<p><font face="Verdana">Fore example:</font></p>
<p><font face="Verdana">#include <string.h> //For strcpy<br>
struct database<br>
{<br>
int age;<br>
char name[20];<br>
float salary;<br>
};</font></p>
<p><font face="Verdana">void main()<br>
{<br>
database employee;<br>
employee.age=22;<br>
strcpy(employee.name, "Joe");<br>
employee.salary= 12000.21;</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">     Don't worry about the name[20].
That is just an array. It can hold more than one character all called under the
same name. They are used like strings. I will do my next lesson on arrays,
I promise, because they are very important. The struct database declares that
database has three variables in it, age, name, and salary.</font></p>
<p><font face="Verdana">     Eventually, you can use
database like a variable type like int. You can create an employee with the
database type like I did above. Then, to modify it you call everything with the
employee. in front of it. You can also return structures from functions by
defining their return type as a structure type. Example:</font></p>
<p><font face="Verdana">     struct database fn();</font></p>
<p><font face="Verdana">     You can make arrays of
structures as well. I will show you how to do this in lesson 8.</font></p>
<p><font face="Verdana">     That will be up in a few days.
I suppose I should explain unions a little bit. They are like structures except
that all the variables share the same memory. When a union is declared the
compiler allocates enough memory for the largest data-type in the union.</font></p>
<p><font face="Verdana">     To access the union you use the
. like in structures. Also, if you are accessing the union of structure through
a pointer use the -> operator. for example, database->employee . The most
useful thing about unions is that you can manipulate the bytes of the
data-types. You might want to see what you can do if you understand that sort of
stuff. Personally, I have never used a union.</font></p>

