## [1] The following function takes two integers as parameters. Make it return a string containing both integers separated by a space. For example, stringify(2, 3) should return '2 3'.

```
String stringify(int x, int y) 

{
  // Return a formatted string here
}
```
## [2] Try putting the ??= and ?? operators to work below.
```
String foo = 'a string';
String bar; // Unassigned objects are null by default.

// Substitute an operator that makes 'a string' be assigned to baz.
String baz = foo /* TODO */ bar;

void updateSomeVars() {
  // Substitute an operator that makes 'a string' be assigned to bar.
  bar /* TODO */ 'a string';
}

```
## [3] Try using conditional property access to finish the code snippet below.
```
// This method should return the uppercase version of `str`
// or null if `str` is null.
String upperCaseIt(String str) {
  // Try conditionally accessing the `toUpperCase` method here.
}

```

## [4] Try setting the following variables to the indicated values.
```
// Assign this a list containing 'a', 'b', and 'c' in that order:
final aListOfStrings = 

// Assign this a set containing 3, 4, and 5:
final aSetOfInts = 

// Assign this a map of String to int so that aMapOfStringsToInts['myKey'] returns 12:
final aMapOfStringsToInts = 

// Assign this an empty List<double>:
final anEmptyListOfDouble = 

// Assign this an empty Set<String>:
final anEmptySetOfString = 

// Assign this an empty Map of double to int:
final anEmptyMapOfDoublesToInts = 

```
## [5] Try finishing the following statements, which use arrow syntax.
```
class MyClass {
  int _value1 = 2;
  int _value2 = 3;
  int _value3 = 5;
  
  // Returns the product of the above values:
  int get product =>
  
  // Adds 1 to _value1:
  void incrementValue1() => 
  
  // Returns a string containing each item in the
  // list, separated by commas (e.g. 'a,b,c'): 
  String joinWithCommas(List<String> strings) =>
}

```
## [6] Imagine you have a shopping cart class that keeps a private List <double> of prices. Add the following:

## *A getter called total that returns the sum of the prices
## *A setter that replaces the list with a new one, as long as the new list doesn’t contain any negative prices (in which case the setter should throw an InvalidPriceException).
```
class InvalidPriceException {}

class ShoppingCart {
  List<double> _prices = [];
  
  // Add a "total" getter here:

  // Add a "prices" setter here:
}

```

## [7] Implement a function called joinWithCommas that accepts one to five integers, then returns a string of those numbers separated by commas. Here are some examples of function calls and returned values:

##Function call	 	                  Returned value
##joinWithCommas(1)	 	                   '1'
##joinWithCommas(1, 2, 3)	            	'1,2,3'
##joinWithCommas(1, 1, 1, 1, 1)	 	    '1,1,1,1,1'
```
String joinWithCommas(int a, [int b, int c, int d, int e]) {

}
```

## [8] Add a copyWith instance method to the MyDataObject class. It should take three named parameters:

## 1. int newInt
## 2. String newString
## 3. double newDouble
##When called, copyWith should return a new MyDataObject based on the current instance, with data from the preceding parameters (if any) copied into the object’s properties. For example, if newInt is non-null, then copy its value into anInt.
```
class MyDataObject {
  final int anInt;
  final String aString;
  final double aDouble;

  MyDataObject({
     this.anInt = 1,
     this.aString = 'Old!',
     this.aDouble = 2.0,
  });

  // Add your copyWith method here:
}

```

## [9] Implement tryFunction below. It should execute an untrustworthy method and then do the following:

## *If untrustworthy throws an ExceptionWithMessage, call logger.logException with the exception type and message (try using on and catch).
## *If untrustworthy throws an Exception, call logger.logException with the exception type (try using on for this one).
## *If untrustworthy throws any other object, don’t catch the exception.
## *After everything’s caught and handled, call logger.doneLogging (try using finally).
```
typedef VoidFunction = void Function();

class ExceptionWithMessage {
  final String message;
  const ExceptionWithMessage(this.message);
}

// Call logException to log an exception, and doneLogging when finished.
abstract class Logger {
  void logException(Type t, [String msg]);
  void doneLogging();
}

void tryFunction(VoidFunction untrustworthy, Logger logger) {
  // Invoking this method might cause an exception. Catch and handle
  // them using try-on-catch-finally.
  untrustworthy();
}

```
## [10] Add a one-line constructor to MyClass that uses this. syntax to receive and assign values for all three properties of the class.
```
class MyClass {
  final int anInt;
  final String aString;
  final double aDouble;
  
  // Create a constructor here.
}

```
## [11] Give the Color class a constructor named Color.black that sets all three properties to zero.
```
class Color {
  int red;
  int green;
  int blue;
  
  Color(this.red, this.green, this.blue);

  // Create a named constructor called "black" here:
}

```
## [12] Modify the Recipe class so its instances can be constants, and create a constant constructor that does the following:
## Has three parameters: ingredients, calories, and milligramsOfSodium (in that order).
## Uses this. syntax to automatically assign the parameter values to the object properties of the same name.
## Is constant, with the const keyword just before Recipe in the constructor declaration.
```
class Recipe {
  List<String> ingredients;
  int calories;
  double milligramsOfSodium;
}

```
