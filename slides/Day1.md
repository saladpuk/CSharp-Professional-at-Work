<!-- .slide: data-auto-animate data-auto-animate-id="bigpicture" -->
## Programming in the BIG picture
> Translate human logic into computer language

🤖 ShowMeWhatYouGot();

---

<!-- .slide: data-auto-animate data-auto-animate-id="bigpicture" -->
## Programming in the BIG picture
1. Fundamentals
1. Solution design
1. Specific problems
1. Facilitators & Tools

> 🧙‍♂️ For any programming languages

===

<!-- .slide: data-auto-animate data-auto-animate-id="datatype" -->
# 🤖
## ShowMeWhatYouGot();
> Memory & Executions

---

<!-- .slide: data-auto-animate data-auto-animate-id="datatype" -->
# 🤖
## ShowMeWhatYouGot();
> Memory & Executions
1. Data types 👈
1. Variables
1. Operators

---

<!-- .slide: data-auto-animate data-auto-animate-id="datatype" -->
## C# Build-in Data types
Common usages
|Group|Keywords|
|--|--|
|Number|<font color="#5799d2">int</font>, <font color="#5799d2">double</font>, <font color="#5799d2">float</font>, <font color="#5799d2">byte</font>, <font color="#5799d2">sbyte</font>, <font color="#5799d2">decimal</font>, <font color="#5799d2">uint</font>, <font color="#5799d2">nint</font>, <font color="#5799d2">nuint</font>, <font color="#5799d2">long</font>, <font color="#5799d2">ulong</font>, <font color="#5799d2">short</font>, <font color="#5799d2">ushor</font>|
|Text|<font color="#5799d2">string, <font color="#5799d2">char</font>|
|Logic|<font color="#5799d2">bool</font>|
|etc|<font color="#5799d2">object</font>, <font color="#5799d2">dynamic</font>|

---

<!-- .slide: data-auto-animate data-auto-animate-id="datatype" -->
## C# Build-in Data types
Common usages

|Group|Keyword|Sample value|
|--|--|--|
|Number|<font color="#5799d2">int</font>|-100, 0, 2000|
||<font color="#5799d2">double</font>|-100.5, 0.66, 2000.345678|
|Text|<font color="#5799d2">string</font>|"Hello", "-1.414", "แมวน้ำ"|
|Logic|<font color="#5799d2">bool</font>|true, false|

---

<!-- .slide: data-auto-animate data-auto-animate-id="datatype" -->
## C# Build-in Data types
Default values
|Type|Default value|
|--|--|
|<font color="#5799d2">Numeric types</font>|0|
|<font color="#5799d2">Reference types</font>|null|
|<font color="#5799d2">bool</font>|false|
|<font color="#5799d2">char</font>|'\0' (U+0000)|

default keyword
```csharp
int number = default; // 0
```
<!-- .element: style="width:38%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="datatype" -->
## C# Build-in Data types
Facilitator functions

```csharp
int.MinValue, int.MaxValue, double.MaxValue, double.MinValue,
double.Epsilon, double.NaN, double.NegativeInfinity,
double.PositiveInfinity, double.IsNegative(),
char.IsDigit(), char.IsLetter(), char.IsAscii(),
string.Join(), string.Concat(), string.IsNullOrWhiteSpace()
```

---

<!-- .slide: data-auto-animate data-auto-animate-id="operatorcs" data-background="white" -->
## Best Practice
🤔 Prevention vs Treatment
```csharp
// Treatment: try-catch statements, validations
int.Parse(), bool.Parse(), double.Parse()
float.Parse(), byte.Parse(), decimal.Parse()
collection.First(), collection.Single()

// Preventions
int.TryParse(), bool.TryParse(), double.TryParse()
float.TryParse(), byte.TryParse(), decimal.TryParse()
collection.FirstOrDefault(), collection.SingleOrDefault()
```
<!-- .element: style="width:80%" -->

===

# 🤖
## ShowMeWhatYouGot();
> Memory & Executions
1. Data types
1. Variables 👈
1. Operators

---

<!-- .slide: data-auto-animate data-auto-animate-id="variable" -->
## Variables
Syntax of variable declaration
> <font color="#5799d2">DataType</font> VariableName;

```csharp [0]
int variable1;
double variable2;
string variable3;
bool variable4;

int apple, banana, coconut;
```
<!-- .element: style="width:45%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="variable" -->
## Variables
1. Names must be a unique name.
1. Names can only contain alpha-numeric characters and underscores but cannot start with a digit.
1. Names are case-sensitive.
1. Reserved words cannot be used as names. except prefix with @ character.
```csharp
int money;
int money;  // ❌ (1) duplicate
int m0n3_y; // ✅ (2)
int 3money; // ❌ (2) start with a number
int Money;  // ✅ (3)
int int;    // ❌ (4) reserved words
int @int;   // ✅ (4)
```
<!-- .element: style="width:60%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="variablesm" data-background="white" -->
## Code smell
> It is any characteristic in the source code of a program that possibly indicates a deeper problem.

🐶 sniff sniff

---

<!-- .slide: data-auto-animate data-auto-animate-id="variablesm" data-background="white" -->
## Code smell
😾 Ambiguous naming
```csharp [0]
double m;      // What's the purpose of it?
double mm;     // What's the difference between them ?
string actpwd; // What's the abbreviation stand for ?
string data;   // Misleading
string generatedSaltValueForEncryptTheAccountPassword; // Hard to read out loud
```
<!-- .element: style="width:110%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="variablesm" data-background="white" -->
## Code smell
😽 Clean code
```csharp [0]
double money;
double minuteOfMeeting;
string accountPassword;
string userData;
string salt4Password;
```
<!-- .element: style="width:40%" -->

===

# 🤖
## ShowMeWhatYouGot();
> Memory & Executions
1. Data types
1. Variables
1. Operators 👈

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
Supported by the built-in types
|Group|Operators|
|--|--|
|1.Arithmetic|++, --, +, -, *, /, %<br/>=, +=, -=, *=, /=, %=|
|2.Comparison|<, >, <=, >=|
|3.Boolean logical|!, &, l, ^, &&, ll, &=, !=, ^= |
|4.Bitwise and shift|<<, >>, >>>, &, l, ^|
|5.Equality|==, !=|

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
Example
```csharp
int moneyInWallet1 = 3;
double moneyInWallet2 = 100.33;
double totalMoney = moneyInWallet1 + moneyInWallet2; // 103.33
bool isRich = totalMoney > 100;                      // true
```

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
Example
```csharp
int moneyInWallet1 = 3;
double moneyInWallet2 = 100.33;
double totalMoney = moneyInWallet1 + moneyInWallet2; // 103.33
bool isRich = totalMoney > 100;                      // true
```

🤔 What's the difference ?
```csharp [0]
int moneyA = 5;
moneyA += ++moneyA + 100; // ???

int moneyB = 5;
moneyB += moneyB++ + 100; // ???
```
<!-- .element: style="width:50%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
&, |, &&, || operators
```csharp [0]
int money = 0;
bool isRich = (money > 0) & (++money >= 2) & (++money >= 2);
Console.WriteLine(money); // ???
```
```csharp [0]
int money = 0;
bool isRich = (money > 0) && (++money >= 2) && (++money >= 2);
Console.WriteLine(money); // ???
```
🤔 What's the difference ?
```csharp [0]
int money = 0;
bool isRich = (money > 0) && (++money >= 2) || (++money >= 2);
Console.WriteLine(money); // ???
```
<!-- .element: class="fragment fade-up" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
⚠️ Round-off errors

```csharp [0]
double a = 3 * 0.1;          // 🤔 0.3
Console.WriteLine(a == 0.3); // Output: false
Console.WriteLine(a - 0.3);  // Output: 5.55111512312578E-17
Console.WriteLine(a);        // Output: 0.30000000000000004

decimal b = 1 / 3m * 3;      // 🤔 1
Console.WriteLine(b == 1);   // Output: false
Console.WriteLine(b);        // Output: 0.99999999999999999
```
It might occur in calculations with floating-point types

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
Grouping by operands
|Group|Example|
|--|--|
|1.Unary|++ -- ~ !|
|2.Binary|+, -, *, /, %<br/>=, +=, -=, *=, /=, %=<br/><, >, <=, >=, ==, !=<br/>&, l, ^, &&, ll<br/>&=, l=, !=, ^=, <<, >>, >>>|
|3.Ternary|?:|

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
[Operator precedence](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/operators/#operator-precedence)
|Priority|Group|Example|
|--|--|--|
|1|Parentheses|()|
|2|Unary|+x, -x, !x, ~x, ++x, --x, ^x|
|3|Multiplicative|x * y, x / y, x % y|
|4|Additive|x + y, x – y|

⚠️ Each row have the same precedence

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
Converting between types

1. Implicit & Explicit conversions
1. Convert class
1. Implicit typing

```csharp [0]
int smallStorage = 3;
double bigStorage;
bigStorage = smallStorage;              // Implicit conversion
smallStorage = (int)bigStorage;         // Explicit conversion

string text;
text = Convert.ToString(bigStorage);    // Convert class
text = Convert.ToString(smallStorage);  // Convert class

var integerStorage = 3;                 // Implicit typing
var floatingStorage = 3.3;              // Implicit typing
```

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
⚠️ Working with numeric types

```csharp
int money = int.MaxValue;
Console.WriteLine(money);        // Output: 2147483647
money++;
Console.WriteLine(money);        // Output: -2147483648
Console.WriteLine(int.MinValue); // Output: -2147483648
```
<!-- .element: style="width:75%" -->
```csharp
Int32 → int (alias)
11111111 11111111 11111111 11111111 =  4,294,967,296
➕➖
01111111 11111111 11111111 11111111 =  2,147,483,647
11111111 11111111 11111111 11111111 = -2,147,483,648

// 🤔 uint.MaxValue + 1 = ???
```
<!-- .element: class="fragment fade-up" style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="operators" -->
## C# Operators
Usage of MaxValue & MinValue
```csharp
long[] numbersToConvert = { 32183, -54000, long.MaxValue / 2 };
foreach (var number in numbersToConvert)
{
    if (number >= int.MinValue && number <= int.MaxValue)
    {
        int newNumber = Convert.ToInt32(number);
        Console.WriteLine($"Successfully converted {newNumber} to an Int32.");
    }
    else
    {
        Console.WriteLine($"Unable to convert {number} to an Int32.");
    }
}

// Output:
// Successfully converted 32183 to an Int32.
// Successfully converted -54000 to an Int32.
// Unable to convert 4611686018427387903 to an Int32.
```
<!-- .element: style="width:105%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="operatorcs" data-background="white" -->
## Code smell
😾 Mystery value
```csharp [0]
int nextPage = -1;
int currentPage = 0;

// Do somthing

if (nextPage != -1)
{
	currentPage += 13;
}
```
<!-- .element: style="width:40%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="operatorcs" data-background="white" -->
## Code smell
😻 Clean code
```csharp [0]
const int InitPage = 0;
const int BlankPage = -1;

int nextPage = BlankPage;
int currentPage = InitPage;

// Do somthing

if (nextPage != BlankPage)
{
	const int PageSize = 13;
	currentPage += PageSize;
}
```
<!-- .element: style="width:50%" -->

===

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
# 🤖 + 🧠
## DecideBasedOnDataAndLogic();
> Decision-making

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
# 🤖 + 🧠
## DecideBasedOnDataAndLogic();
> Decision-making
1. if statements 👈
1. switch statements
1. while statements
1. for statements

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
CONDITION = ✅ | ❌
```csharp [0|1|2-4|4|6|1|6]
if ( CONDITIONS )
{
	// ✅ Valid
}

Next statement
``` 
<!-- .element: style="width:35%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
Example 1 - The condition is valid ✅
```csharp [0|1|2|3-6|6|8]
int age = 20;
if ( age >= 18 )
{
	age += 50;
	age += 10;
}

Console.WriteLine(age); // Output: 80
```
<!-- .element: style="width:60%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
Example 2 - The condition is invalid ❌
```csharp [0|1|2|8]
int age = 12;
if ( age >= 18 )
{
	age += 50;
	age += 10;
}

Console.WriteLine(age); // Output: 12
``` 
<!-- .element: style="width:60%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
Example 3 - Group of conditions
```csharp [0|1-2|3|4-7|7|9-10]
int age = 20;
int money = 1000;
if ( age >= 18 && money >= 300 )
{
	age += 60;
	money -= 300;
}

Console.WriteLine(age);   // Output: 80
Console.WriteLine(money); // Output: 700
```
<!-- .element: style="width:65%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
else statement
```csharp [0|1|2-4|4|10|1|5-8|8|10]
if ( CONDITIONS )
{
	// ✅ Valid
}
else
{
	// ❌ Invalid
}

Next statement
```
<!-- .element: style="width:40%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
Example 4 - The condition is valid ✅
```csharp [0|1|2|3-6|6|13]
int age = 20;
if ( age >= 18 )
{
	age += 50;
	age += 10;
}
else
{
	age += 2;
	age += 3;
}

Console.WriteLine(age); // Output: 80
```
<!-- .element: style="width:60%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
Example 5 - The condition is invalid ❌
```csharp [0|1|2|7-11|11|13]
int age = 12;
if ( age >= 18 )
{
	age += 50;
	age += 10;
}
else
{
	age += 2;
	age += 3;
}

Console.WriteLine(age); // Output: 17
```
<!-- .element: style="width:60%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
else-if statement
```csharp [0|1|2-4|4|15|1|5|6-8|8|15|1|5|9|10-13|13|15]
if ( CONDITIONS-1 )
{
	// ✅ CONDITIONS-1 is valid
}
else if ( CONDITIONS-2 )
{
	// ✅ CONDITIONS-2 is valid
}
// else-if statements ...
else
{
	// ❌ All conditions above are invalid
}

Next statement
```
<!-- .element: style="width:70%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
Nested if statment
```csharp [0|1|2-11|3|4-6|6|13|3|7-10|10|13]
if ( CONDITIONS-1 )
{
	if ( CONDITION-2 )
	{
		// ✅ CONDITIONS-1 AND CONDITION-2 are valid
	}
	else
	{
		// ✅ CONDITIONS-1 is valid but CONDITION-2 is invalid
	}
}

Next statement
``` 

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
Blocks is an optional
```csharp [0|1|2|6|1|3-4|6]
if ( CONDITIONS )
	// Statement A
else
	// Statement B

Next statement
```
<!-- .element: style="width:40%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
Short if statement
```csharp [0]
int money = 0;
if ( money <= 100 )
{
	money += 20;
}
else
{
	money += 1;
}

Console.WriteLine(money); // Output: 20
``` 
<!-- .element: style="width:60%" -->
Full if-else statement
---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelse" -->
## if statements
Short if statement
> CONDITION? OnValid : OnInvalid;
```csharp [0|1|2|3]
int money = 0;
money += money <= 100? 20 : 1;
Console.WriteLine(money); // Output: 20
```
<!-- .element: style="width:60%" -->
Ternary operator

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelsecs" data-background="white" -->
## Code smell
😾 Bad code - Indent Hadouken
```csharp [0]
if ( CONDITIONS-1 )
{
	if ( CONDITION-2 )
	{
		if ( CONDITION-3 )
		{
			if ( CONDITION-4 )
			{
				// Do something
			}
		}
	}
}
``` 
<!-- .element: style="width:60%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelsecs" data-background="white" -->
## Code smell
😺 Good code
```csharp [0]
if ( CONDITIONS-1 && CONDITIONS-2 && CONDITIONS-3 )
{
	// Do something
}
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelsecs" data-background="white" -->
## Code smell
😾 Bad code - Hard to understand the intention
```csharp [0]
if ( CONDITIONS-1 && CONDITIONS-2 && CONDITIONS-3
		&& ( VariableA >= 3 || CONDITIONS-4 ) && !CONDITION-5
		|| ( CONDITION-7 && CONDITIONS-8 && CONDITION-9 ))
{
	// 🤔 For what?
}
else if ( !CONDITION-1 && CONDITION-4 && CONDITION-11 
	|| CONDITION-7 && !( CONDITION-2 && !CONDITION-5 ))
{
	// 😵‍💫 Is this block necessary ?
}
else
{
	// 😱 Required understand all of the conditions above
}
```

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelsecs" data-background="white" -->
## Code smell
😻 Clean code
```csharp [0]
var isAdmin = CONDITIONS-1 && CONDITIONS-2 && CONDITIONS ... ;
var isMod = !CONDITION-1 && CONDITION-4 && CONDITIONS ... ;

if ( isAdmin )
{
	// Do admin stuff
}
else if ( isMod )
{
	// Do moderator stuff
}
else
{
	// Do user stuff
}
```
Clear intentions
---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelsecs" data-background="white" -->
## Code smell
😾 Bad code - Misunderstanding
```csharp [0]
var isNotAdmin = !(CONDITIONS-1 && CONDITIONS ... );
if ( !isNotAdmin )
{
	// 🤔 Admin ??
}
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelsecs" data-background="white" -->
## Code smell
😾 Bad code - Misunderstanding
```csharp [0]
// 😵‍💫 ???
var extraValue = CONDITION1? 10 : CONDITION2? 
	CONDITION3? 20 : 30 : CONDITION4? CONDITION5? 40 : 50 : 60;
```

---

<!-- .slide: data-auto-animate data-auto-animate-id="ifelsecs" data-background="white" -->
## Clean code
💖 Maintainable code by eliminating complexities

===

# 🤖 + 🧠
## DecideBasedOnDataAndLogic();
> Decision-making
1. if statements
1. switch statements 👈
1. while statements
1. for statements

---

<!-- .slide: data-auto-animate data-auto-animate-id="switch" -->
## switch statements
```csharp [0|1|3|4-7|6|15|1|8|9-12|11|15]
switch ( DATA )
{
	case VALUE1:
	{
		// ✅ DATA == VALUE1
		break;
	}
	default:
	{
		// ❌ Data does not match with any cases
		break;
	}
}

Next statement
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="switch" -->
## switch statements
```csharp [0|1|3|8|9-12|11|20]
switch ( "Banana" )
{
	case "Apple":
	{
		// Do Apple stuff
		break;
	}
	case "Banana":
	{
		// Do Banana stuff
		break;
	}
	default:
	{
		// Do default stuff
		break;
	}
}

Next statement
```
<!-- .element: style="width:60%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="switch" -->
## switch statements
```csharp [0|1|3|8|13|14-17|16|20]
switch ( "XXXX" )
{
	case "Apple":
	{
		// Do Apple stuff
		break;
	}
	case "Banana":
	{
		// Do Banana stuff
		break;
	}
	default:
	{
		// Do default stuff
		break;
	}
}

Next statement
```
<!-- .element: style="width:60%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="switch" -->
## switch statements
Combinations & Evaluations
```csharp [0|1|6|7|10|11-13|13|15|0]
switch ( "Coconut" )
{
	default:
		// Do default stuff
		break;
	case "Apple": 
	case "Banana":
		// Do Apple & Banana stuff
		break;
	case "Coconut":
		// Do Coconut stuff
		break;
}

Next statement
```
<!-- .element: style="width:60%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="selectioncompare" -->
## if ⚔️ switch
🤔 What's the difference ?

---

<!-- .slide: data-auto-animate data-auto-animate-id="selectioncompare" -->
## if ⚔️ switch
C# Pattern matching
```csharp
object position = new Point(5, 10);
```
<!-- .element: style="width:50%" -->
```csharp [0]
// if
if (position is Point p && p.X == p.Y && p.X > 0 && p.X <= 100)
{
	// Do something
}
```
```csharp [0]
// switch
switch (position)
{
	case Point p when p.X == p.Y && p.X > 0 && p.X <= 100:
		// Do point stuff
		break;
	default:
		// Do default stuff
		break;
}
```

===

# 🤖 + 🧠
## DecideBasedOnDataAndLogic();
> Decision-making
1. if statements
1. switch statements
1. while statements 👈
1. for statements

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while statements
```csharp [0|1|2-4|4|1|2-4|4|6]
while ( CONDITIONS )
{
	// ✅ Valid
}

Next statement
``` 
<!-- .element: style="width:40%" -->
Repeat until the condition is invalid

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while statements
Example 1 - The condition is valid ✅
```csharp [0|1|2|3-6|4|5|6|2|3-6|4|5|6|2|3-6|4|5|6|2|8]
int counter = 3;
while ( counter > 0 )
{
	Console.WriteLine(counter); // Output: 3, 2, 1
	counter--;
}

Next statement
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while statements
Example 2 - The condition is invalid ❌
```csharp [0|1|2|8]
int counter = -1;
while ( counter > 0 )
{
	Console.WriteLine(counter);
	counter--;
}

Next statement
```
<!-- .element: style="width:50%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while statements
break keyword
```csharp [0|1|2|3-7|4|5|7|9]
int counter = 3;
while ( counter > 0 )
{
	Console.WriteLine(counter); // Output: 3
	break;
	counter--;
}

Console.WriteLine(counter);     // Output: 3
```
<!-- .element: style="width:65%" -->
One statement to rule them all 💍

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while statements
continue keyword
```csharp [0|1|2|3-10|4|5|9|10|2|4|5|7|2|4|5|9|10|2|12]
int counter = 0;
while ( counter < 3 )
{
    counter++;
    if ( counter % 2 == 0 )
    {
        continue;
    }
    Console.WriteLine(counter); // Output: 1, 3
}

Next statement 
```
<!-- .element: style="width:70%" -->
🥴 Go home you're drunk

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while statements
do-while statement
```csharp [0|1-4|4|5|2-4|4|5|2-4|4|5|7]
do
{
	// ✅ First time or conditions is valid
}
while ( CONDITIONS );

Next statement
``` 
<!-- .element: style="width:70%" -->
while loop with free trial


---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while loop statements
Example 3 - The condition is valid ✅
```csharp [0|1|3-6|7|4-6|7|4-6|7|9]
var counter = 3;

do
{
	Console.WriteLine(counter--); // Output: 3, 2, 1
}
while ( counter > 0 );

Next statement
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while loop statements
Example 4 - The condition is invalid ❌
```csharp [0|1|3-6|7|9]
var counter = 3;

do
{
	Console.WriteLine(counter--); // Output: 3
}
while ( counter > 0 );

Next statement
```
<!-- .element: style="width:70%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while loop statements
Scenario - Retrieve data for the first time
```csharp [0|1-2|4-8|6|7|8|9|5-8|6|7|8|9|11]
var currentPage = 0;
var hasNextPage = false;

do
{
	// Send the current page to retrieve data from the server.
	hasNextPage = data.NextPage > -1;
}
while ( hasNextPage );

Next statement
```

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while loop statements
Block is an option
```csharp [0|1|2|3|2|3||2|3|5]
var counter = 3;
while ( counter > 0 );
	Console.WriteLine(counter--); // Output: 3, 2, 1

Next statement
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="while" -->
## while loop statements
Block is an option
```csharp [0|1|2-3|4|2-3|4|2-3|4|6]
var counter = 3;
do
	Console.WriteLine(counter--); // Output: 3, 2, 1
while ( counter > 0 );

Next statement
```
<!-- .element: style="width:75%" -->

===

# 🤖 + 🧠
## DecideBasedOnDataAndLogic();
> Decision-making
1. if statements
1. switch statements
1. while statements
1. for statements 👈

---

<!-- .slide: data-auto-animate data-auto-animate-id="for" -->
## for statements
```csharp [0|1|2-4|3|4|1|2-4|3|4|1|6]
for ( INITIALIZER ; CONDITIONS ; ITERATOR )
{
	// ✅ Valid
}

Next statement
``` 
<!-- .element: style="width:70%" -->
while loop with facilitators

---

<!-- .slide: data-auto-animate data-auto-animate-id="for" -->
## for statements
Example 1 - The condition is valid ✅
```csharp [0|1|2-4|3|4|1|2-4|3|4|1|6]
for ( int counter = 3 ; counter > 0 ; counter-- )
{
	Console.WriteLine(counter); // Output: 3, 2, 1
}

Next statement
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="for" -->
## for statements
Example 2 - The condition is invalid ❌
```csharp [0|1|6]
for ( int counter = -1 ; counter > 0 ; counter-- )
{
	Console.WriteLine(counter);
}

Next statement
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="for" -->
## for statements
Initializer & Iterator blocks are optional
```csharp [0|1|2|3-5|5|2|3-5|5|2|3-5|5|2|7]
int counter = 3;
for (  ; counter > 0 ;  )
{
	Console.WriteLine(counter--);  // Output: 3, 2, 1
}

Next statement
```
<!-- .element: style="width:80%" -->
🤔 while ?

---

<!-- .slide: data-auto-animate data-auto-animate-id="iterationcompare" -->
## while ⚔️ for
🤔 What's the difference ?

---

<!-- .slide: data-auto-animate data-auto-animate-id="iterationcompare" -->
## while ⚔️ for
🤔 What's the difference ?

```csharp
int counter = 3;
while ( counter > 0 )
{
	// Do something
}
```
<!-- .element: style="width:70%" -->
```csharp
int counter = 3;
do
{
	// Do something
} while ( counter > 0 );

```
<!-- .element: style="width:70%" -->
```csharp
for ( int counter = 3; counter > 0; counter-- )
{
	// Do something
}
```
<!-- .element: style="width:70%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="iterationcompare" -->
## goto statement
Syntax of method declaration
> LabelName:
```csharp [0|1|2|5|6|7]
int money = 10;
goto Line5;
money = 200;

Line5:
money++;
Console.WriteLine(money); // Output: 11
```
<!-- .element: style="width:60%" -->
🦘 Portal

---

<!-- .slide: data-auto-animate data-auto-animate-id="iterationcompare" -->
## goto statement
goto loop
```csharp [0|1|2|3|7|8|2|3|7|8|2|3|7|8|2|3|5|10|11|0]
int counter = 0;
TryAgain:
if (counter >= 3)
{
    goto Exit;
}
counter++;
goto TryAgain;

Exit:
Console.WriteLine(counter);  // Output: 3
```
<!-- .element: style="width:70%" -->
🥴 Avoid using goto statements

===

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
# 📰 → 📃📃📃
## Methods();
> Separate one large block

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
# 📰 → 📃📃📃
## Methods();
> Separate one large block
1. Return values
1. Parameters & Arguments
1. Scope of parameters
1. Recursive calls

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
Syntax of method declaration
> <font color="#5799d2">ReturnType</font> MethodName( <font color="#4ec9b0">Parameters</font> ) { }
<!-- .element: style="width:100%" -->
---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
Syntax of method declaration
> <font color="#5799d2">ReturnType</font> MethodName( <font color="#4ec9b0">Parameters</font> ) { }
<!-- .element: style="width:100%" -->

```csharp [0|1-4|6-9|11|11,1-4|11|12|12,6-9|12]
int GetNumber()
{
	return 99;                   // int
}

string GetGreeting()
{
	return "Hello world!";       // string
}

int number = GetNumber();        // 99
string message = GetGreeting();  // "Hello world"
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
void keyword
```csharp [0|1-6|8|8,1-6|3|4|6|8|9]
void ClearHistories()
{
	// Clean stuff
	return;
	// Abandoned statements
}

ClearHistories();
var result = ClearHistories(); // ❌ Compile error
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
Parameters & Arguments

```csharp [0|1-4|6-9|11|11,1-4|11|12|12,6-9|8|12]
void Print(string message)
{
	Console.WriteLine(message);
}

int Add(int firstValue, int secondValue)
{
	return firstValue + secondValue;
}

Print("Hello world!");      // Output: Hello world!
int result = Add(100, 20);  // 120
```
<!-- .element: style="width:75%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
Scope of parameters
```csharp [0|1,3-7|9|9,3-7|5|5,3|6|6,3|9|10|10,1]
int money = 5;

void Add100AndPrint(int money)
{
	money += 100;             // 105
	Console.WriteLine(money); // Output: 105
}

Add100AndPrint(money);
Console.WriteLine(money);     // Output: 5
```
<!-- .element: style="width:70%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
this keyword
```csharp [0|1,3-7|9|9,3-7|5|5,1|6|6,3|9|10|10,1]
int money = 5;

void Add100AndPrint(int money)
{
	this.money += 100;        // 105
	Console.WriteLine(money); // Output: 5
}

Add100AndPrint(money);
Console.WriteLine(money);     // Output: 105
```
<!-- .element: style="width:70%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
Default parameters
```csharp [0|1-4|1|6|6,1|6,3|6|7|7,1|7,3|7]
void Print(string message = "Hi")
{
	Console.WriteLine(message);
}

Print();                // Output: Hi
Print("Hello world!");  // Output: Hello world!
```
<!-- .element: style="width:70%" -->

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
Return Tuple types
```csharp [0|1-7|9|1-7|3|4|5|6|9|1,6,10|1,6,11]
(bool, double) Withdraw(int amount)
{
	// Do withdrawal stuff
	bool isSuccess = transaction.Result;
	double balanceRemaining = transaction.Balance;
	return (isSuccess, balance);
}

var result = Withdraw(100);
Console.WriteLine(result.Item1); // Is success
Console.WriteLine(result.Item2); // Balance remaining
```
<!-- .element: style="width:80%" -->
Lightweight data structure

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
Recursive method
```csharp [0]
void MethodA()
{
    MethodA();
}
```
<!-- .element: style="width:40%" -->
Making a function call itself

---

<!-- .slide: data-auto-animate data-auto-animate-id="methods" -->
## Methods
Example 5!
> N Factorial = 1 x 2 x 3 x ... x N
```csharp [0|1-9|11|11,1|3|8|1|3|8|1|3|8|1|3|5|8|11]
int Factorial(int value)
{
	if( value <= 1 )
	{
		return value;
	}

	return value * Factorial(--value);
}

var result = Factorial(4); // 24 = 1 x 2 x 3 x 4
```
<!-- .element: style="width:75%" -->
💀 C# is not good at recursive.

---

<!-- .slide: data-auto-animate data-auto-animate-id="methodscs" data-background="white" -->
## Code smell
### Needless Complexity
```csharp [0]
int Factorial(int value)
{
	int result = 1;
	for (int i = 1; i <= value; i++)
	{
		result *= i;
	}
	return result;
}

var result = Factorial(4); // 24 = 1 x 2 x 3 x 4
```
<!-- .element: style="width:75%" -->
😻 Simple is the best

---

<!-- .slide: data-auto-animate data-auto-animate-id="methodscs" data-background="white" -->
## Code smell
😾 Ambiguous naming
```csharp [0]
AccountNameChanger(string name)              // Boring to read
CreateAccount(string uName, string pwd, ...) // Hard to use
ChangeAccountPasswordAndDeleteIfNotValid()   // Why delete ? 
```

---

<!-- .slide: data-auto-animate data-auto-animate-id="methodscs" data-background="white" -->
## Code smell
😾 Ambiguous naming
```csharp [0]
AccountNameChanger(string name)              // Boring to read
CreateAccount(string uName, string pwd, ...) // Hard to use
ChangeAccountPasswordAndDeleteIfNotValid()   // Why delete ? 
```

😻 Clean code
```csharp [0]
ChangeAccountName(string name)
CreateAccount(AccountInfo account)
ChangeAccountPassword()
DeleteAccountIfNoBirthDate()
```
<!-- .element: style="width:55%" -->

---

<!-- .slide: data-background="pink" -->
## 💖 SOLID Design Principles
### Single-Responsibility Principle
> Class, Method, Module should have only one reason to change.

===

# 🎮 Challenge
## 🧮 Calculator

===

## Summary
1. 🤖 Data & Operations
1. 🤖 + 🧠 Decision-making
1. 📰 → 📃📃📃 Methods

> 💖 Code design