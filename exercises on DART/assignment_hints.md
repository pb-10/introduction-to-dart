## HINT #1:

-Both x and y are simple values, and Dart's string interpolation will handle converting them to string representations. All you need to do is use the $ operator to reference them inside single quotes, with a space in between.

## HINT for #2:

-All you need to do in this exercise is replace the TODO comments with either ?? or ??=. Read the codelab text to make sure you understand both, and then give it a try.

## HINT for #3:

-If this exercise wanted you to conditionally lowercase a string, you could do it like this: str?.toLowerCase()

## HINT for #4:

-This exercise is fairly straightforward. Just add a list, set, or map literal after each equals sign. See the codelab text for the correct syntax to use.

## HINT for #5:

-For the product, you can just multiply the three values together. For incrementValue1, you can use the increment operator (++). For joinWithCommas, try using the join method found in the List class.

## HINT for #6:

-There are two functions that come in handy for this exercise. One is `fold`, which can reduce a list to a single value (try it to calculate the total). The other is `any`, which can check each item in a list with a function you give it (try using it to check if there are any negative prices in the prices setter).

## HINT for #7:

-The b, c, d, and e paramters will be null if they aren't provided by caller. The important thing, then, is to check whether those arguments are null before you add them to the final string.

## HINT for #8:

-The copyWith method shows up in a lot of classes and libraries. Yours should do a few things: use optional named parameters, create a new instance of MyDataObject, and use the data from the parameters to fill it (or the data from the current instance if the parameters are null. This is a chance to get more practice with the ?? operator!

## HINT for #9:

-This exercise looks tricky, but it's really one big `try` statement. Just call `untrustworthy` inside the `try`, and then use `on`, `catch`, and `finally` to catch exceptions and call methods on the logger.

## HINT for #10:

-This exercise has a one line solution. Just declare the constructor with `this.anInt`, `this.aString`, and `this.aDouble` as its parameters in that order.

## HINT for #11:

-The declaration for your constructor should be `Color.black() {}`. Inside the braces, set red, green, and blue to zero.

## HINT for #12:
 
-In order to make the constructor const, you'll need to make all the properties final.