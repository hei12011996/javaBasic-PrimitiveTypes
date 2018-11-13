## BooleanOperatorsTest
- should_perform_logical_boolean_operations()
1. The knowledge point of this unit test is to know the result of each boolean logical operators including &&, ||, &, |, ==, !=. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/operators.html
2. The original expected result is empty at first.
3. For && and &, its result will only be true if the results of both sides are true, otherwise it is false. For || and |, its result will be true if either side result is true, otherwise it will be false if the results of both sides are false. For ==, it will be true if the result of both sides are equal. For !=, it will be true if the result of both sides are not equal.
4. No

- should_do_bitwise_and_boolean_operation()
1. The knowledge point of this uni test is to know the result of bitwise and operator. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op3.html
2. The original expected result is filled as zero at first.
3. It is executing a bitwise and operation for each bit of the integer, for 0x1234_abcd and 0x000f_ff00, we just keep the bit of first integer that is at the same position of 'f' of the sceond integer, while keep the bit as zero if the bit of that position of either integer is zero, should the result should be 0x0004_ab00.
4. No

- should_do_bitwise_or_boolean_operation()
1. The knowledge point of this uni test is to know the result of bitwise or operator. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op3.html
2. The original expected result is filled as zero at first.
3. It is executing a bitwise or operation for each bit of the integer, for 0x1234_0000 and 0x0000_abcd, we keep the bit which is not zero on both sides of the same position, so the result should be 0x1234_abcd.
4. No

- should_do_bitwise_not_operation()
1. The knowledge point of this uni test is to know the result of bitwise not operator. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op3.html
2. The original expected result is zero at first.
3. It is executing a bitwise not operation for each bit of the integer, which invert the bit digit. So if we meet 'f', we change it to '0', if we meet '0', change it to 'f'. So for integer 0x0000_ffff, the result should be 0xffff_0000.
4. No

## CharTypeTest
- should_describe_escaped_chars()
1. The knowledge point of this unit test is to know the use of escape characters. Offical document: https://docs.oracle.com/javase/tutorial/java/data/characters.html
2. The original expected results are all space chacters at first.
3. In order to represent some special characters which have speical meaning, a backslash is needed be put in front of the character that needed to be escape(e.g " -> \"). For backspace, tab, linefeed, and carriageReturn, there are also escape sequence to represent such characters, for instance \b for backspace, \t for tab, \n for linefeed, \r for carriageReturn.
4. No

## FloatingTypeTest
- should_not_get_rounded_result_if_convert_floating_number_to_integer()
1. The knowledge point of this unit test is to know the result of down casting. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html
2. The original expected result is Integer.MAX_VALUE, which is even larger than the floating number 2.75.
3. The true result should be 2 as down casting a float number will cause it lose the value after decimal point.
4. No

- should_judge_special_double_cases()
1. The knowledge point of this unit test is to use some Java provided method to determine some special or invalid number of double like divided by zero. Offical document: https://docs.oracle.com/javase/8/docs/api/java/lang/Double.html
2. The original function isNan() and isInfinity() are not yet implemented and throw a NotImplementedException.
3. Call Double.isNaN() and Double.isInfinite() for method isNan() and isInfinity() which are called in should_judge_special_double_cases().
4. No

- should_not_round_number_when_convert_to_integer()
1. The knowledge point of this unit test is to know the result of down casting. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html
2. The original expected result is Integer.MAX_VALUE, which is even larger than the floating number 2.75.
3. The true result should be 2 as down casting a float number will cause it lose the value after decimal point.
4. No

- should_round_number()
1. The knowledge point of this unit test is to use some Java provided method to round double. Offical document: https://docs.oracle.com/javase/tutorial/java/data/beyondmath.html
2. The original expected result is Integer.MAX_VALUE, which is even larger than the floating number 2.75.
3. Call Math.round() in order to round a double to long.
4. No

## IntegerTypeTest
- should_get_range_of_primitive_int_type()
1. The knowledge point of this unit test is to know that maximum value and minimum value of an int, which a Java class Integer also store these values as constant. Offical document: https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html
2. The original expected results are both filled 0 for maximum and minimum.
3. Put Integer.MAX_VALUE and Integer.MIN_VALUE in the expected result.
4. No

- should_get_range_of_primitive_short_type()
1. The knowledge point of this unit test is to know that maximum value and minimum value of a short, which a Java class Short also store these values as constant. Offical document: https://docs.oracle.com/javase/8/docs/api/java/lang/Short.html
2. The original expected results are both filled 0 for maximum and minimum.
3. Put Short.MAX_VALUE and Short.MIN_VALUE in the expected result.
4. No

- should_get_range_of_primitive_long_type()
1. The knowledge point of this unit test is to know that maximum value and minimum value of a long, which a Java class Long also store these values as constant. Offical document: https://docs.oracle.com/javase/8/docs/api/java/lang/Long.html
2. The original expected results are both filled 0 for maximum and minimum.
3. Put Long.MAX_VALUE and Long.MIN_VALUE in the expected result.
4. No

- should_get_range_of_primitive_byte_type()
1. The knowledge point of this unit test is to know that maximum value and minimum value of a byte, which a Java class Byte also store these values as constant. Offical document: https://docs.oracle.com/javase/8/docs/api/java/lang/Byte.html
2. The original expected results are both filled 0 for maximum and minimum.
3. Put Byte.MAX_VALUE and Byte.MIN_VALUE in the expected result.
4. No

- should_overflow_silently()
1. The knowledge point of this unit test is to know that the effect of ++ operator and what happen when a number overflow, which will go to the minimum value when adding one to a maximum value. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html
2. The original expected result is filled as 0 at first.
3. Put Integer.MIN_VALUE as expected result as it is the result of adding one to INTEGER.MAX_VALUE.
4. No

- should_throw_exception_when_overflow()
1. The knowledge point of this unit test is to use the Java provided Method to perform a add operation, which will check overflow situation and throw exception in such case. Offical document: https://docs.oracle.com/javase/8/docs/api/java/lang/Math.html
2. The original function add() is not yet implemented and throw a NotImplementedException.
3. Called Math.addExact() in method add() which is called in should_throw_exception_when_overflow(), thus it will throw ArithmeticException when underflow or overflow happens. 
4. No

- should_take_care_of_number_type_when_doing_calculation()
1. The knowledge point of this unit test is to know the result of a operation will have its own data type if not specify by programmer, and thus the operation like 2 / 3 will result in 0 as its type is int, which may affect the final result is not what the programmer expect. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op1.html
2. The original expected results are filled as Double.POSITIVE_INFINITY at first.
3. For the first result for 2 / 3 * 5 will first calculate the 2 / 3, which result is 0 for int, then 0 * 5 is 0. So the first expected result is 0. While the second result for 2 * 5 / 3 will first calculate 2 * 5 = 10, while 10 / 3 is 3 for int (dropping the value 0.33333 after decimal point as it is int), so the second expected result should be 3.
4. No

- should_truncate_number_when_casting()
1. The knowledge point of this unit test is to know the difference between integer and short. Int can store a 32-bit integer while short can only store a 16-bit integer. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html
2. The original expected result is filled as 0.
3. The integer is having the value 0x0123_4567, while that 0123_4567 is each 4 bit value, casting it to short will cause it lost the value which exceed it store limit, so it can only store the part for 4567 for a short. So the expected result should be 0x4567
4. No

- should_increment()
1. The knowledge point of this unit test is to know the effect of ++ operator. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op1.html
2. The original expected results are both filled as 0.
3. The result is integer++, which increment happens after the assignment. So for the currentInteger value, it would be 4, while the result is only 3 as it is assigned the value of variable "integer" before increment.
4. No

- should_increment_2()
1. The knowledge point of this unit test is to know the effect of ++ operator. Offical document: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op1.html
2. The original expected results are both filled as 0.
3. The result is ++integer, which increment happens before the assignment. So for the currentInteger value, it would be 4, while the result is also 4 as it is assigned the value of variable "integer" after increment.
4. No
