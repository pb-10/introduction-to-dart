##Solution for #1:
```
String stringify(int x, int y) {
  return '$x $y';
}
```


##Solution for #2:
```
String foo = 'a string';
String bar; // Unassigned objects are null by default.

// Substitute an operator that makes 'a string' be assigned to baz.
String baz = foo ?? bar;

void updateBar() {
  // Substitute an operator that makes 'a string' be assigned to bar.
  bar ??= 'a string';
}
```


##Solution for #3:
```
// This method should return the uppercase version of `str`
// or null if `str` is null.
String upperCaseIt(String str) {
  return str?.toUpperCase();
}
```


##Solution for #4:
```
// Assign this a list containing 'a', 'b', and 'c' in that order:
final aListOfStrings = ['a', 'b', 'c'];

// Assign this a set containing 3, 4, and 5:
final aSetOfInts = {3, 4, 5};

// Assign this a map of String to int so that aMapOfStringsToInts['myKey'] returns 12:
final aMapOfStringsToInts = {'myKey': 12};

// Assign this an empty List<double>:
final anEmptyListOfDouble = <double>[];

// Assign this an empty Set<String>:
final anEmptySetOfString = <String>{};

// Assign this an empty Map of double to int:
final anEmptyMapOfDoublesToInts = <double, int>{};
```


##Solution for #5:
```
class MyClass {
  int _value1 = 2;
  int _value2 = 3;
  int _value3 = 5;

  // Returns the product of the above values:
  int get product => _value1 * _value2 * _value3;
  
  // Adds one to _value1:
  void incrementValue1() => _value1++; 
  
  // Returns a string containing each item in the
  // list, separated by commas (e.g. 'a,b,c'): 
  String joinWithCommas(List<String> strings) => strings.join(',');
}
```


##Solution for #6:
```
class InvalidPriceException {}

class ShoppingCart {
  List<double> _prices = [];
  
  double get total => _prices.fold(0, (e, t) => e + t);
  
  set prices(List<double> value) {
    if (value.any((p) => p < 0)) {
      throw InvalidPriceException();
    }
    
    _prices = value;
  }
}
```


##Solution for #7
```
String joinWithCommas(int a, [int b, int c, int d, int e]) {
  var total = '$a';
  if (b != null) total = '$total,$b';
  if (c != null) total = '$total,$c';
  if (d != null) total = '$total,$d';
  if (e != null) total = '$total,$e';
  return total;
}
```


##Solution for #8:
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

  MyDataObject copyWith({int newInt, String newString, double newDouble}) {
    return MyDataObject(
      anInt: newInt ?? this.anInt,
      aString: newString ?? this.aString,
      aDouble: newDouble ?? this.aDouble,
    );
  }
}
```


## Solution for #9:
```
typedef VoidFunction = void Function();

class ExceptionWithMessage {
  final String message;
  const ExceptionWithMessage(this.message);
}

abstract class Logger {
  void logException(Type t, [String msg]);
  void doneLogging();
}

void tryFunction(VoidFunction untrustworthy, Logger logger) {
  try {
    untrustworthy();
  } on ExceptionWithMessage catch (e) {
    logger.logException(e.runtimeType, e.message);
  } on Exception {
    logger.logException(Exception);
  } finally {
    logger.doneLogging();
  }
}
```


## Solution for #10:
```
class MyClass {
  final int anInt;
  final String aString;
  final double aDouble;
  
  MyClass(this.anInt, this.aString, this.aDouble);
}
```


## Solution for #11:
```
class Color {
  int red;
  int green;
  int blue;
  
  Color(this.red, this.green, this.blue);

  Color.black() {
    red = 0;
    green = 0;
    blue = 0;
  } 
}
```


## Solution for #12:
```
class Recipe {
  final List<String> ingredients;
  final int calories;
  final double milligramsOfSodium;

  const Recipe(this.ingredients, this.calories, this.milligramsOfSodium);
}
```
