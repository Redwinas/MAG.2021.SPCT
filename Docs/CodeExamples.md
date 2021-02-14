# Code examples

Here are provided 3 code examples:

* [Converter Example with Int](#example_1)
* [Converter Example with String](#example_2)
* [TypeConerter Example](#example_3)

### Converter Example code

<a name="example_1"></a>
#### Example with Int

```c#
private static void ConverterExample_WithInt()
        {
            Converter conv = new Converter(125); // Create converter with 125 value

            String convFullData = conv.ToFullString(); // Gets object's value's all data as string
            String convFullDataWithSpaces = conv.ToFullString(3); // Gets object's value's all data as string and adds space between elemetns
            String convFullDataWithCharSpaces = conv.ToFullString(3, '-'); // Gets object's value's all data as string and adds char symbol between elements

            Console.WriteLine("--------------------");
            Console.WriteLine(convFullData);
            Console.WriteLine("--------------------");
            Console.WriteLine(convFullDataWithSpaces);
            Console.WriteLine("--------------------");
            Console.WriteLine(convFullDataWithCharSpaces);
            Console.WriteLine("--------------------");

            List<Char> binaryList = conv.ToBinaryArray(); // Return value as Binary value in List<Char> format
            List<Char> hexList = conv.ToHexArray(); // Return value as Hex value in List<Char> format
            List<Char> octalList = conv.ToOctalArray(); // Return value as Octal value in List<Char> format
            List<Char> decList = conv.ToDecArray(); // Return value as Decimal value in List<Char> format

            String savedValue = conv.ToString(); // Returns set value as string

            Console.WriteLine("--------------------");
            Console.WriteLine("Object's value: " + savedValue);
            Console.WriteLine("Binary List printed: [" + String.Join(", ", binaryList) + "]");
            Console.WriteLine("Hex List printed: [" + String.Join(", ", hexList) + "]");
            Console.WriteLine("Octal List printed: [" + String.Join(", ", octalList) + "]");
            Console.WriteLine("Dec List printed: [" + String.Join(", ", decList) + "]");
            Console.WriteLine("--------------------");


            String valueBeforeChange = conv.ToString(); // Gets current value
            String valueBeforeChangeHex = conv.ToHexString(); // Gets current value in hex format

            String replace = conv.ReplaceHex("d", "fdf"); // Replaces Hex value's 65 with 44 making our Example to ExamplD
            String valueAfterChange = conv.ToString(); // Gets new value

            // Prints out values
            Console.WriteLine("--------------------");
            Console.WriteLine("Value before change: " + valueBeforeChange);
            Console.WriteLine("Value before change(Hex): " + valueBeforeChangeHex);
            Console.WriteLine("Returned value: " + replace);
            Console.WriteLine("Value after change: " + valueAfterChange);
            Console.WriteLine("--------------------");


            valueBeforeChange = conv.ToString(); // Gets current value
            valueBeforeChangeHex = conv.ToHexString();

            String addedVal = conv.AddVal("12", 1); // Inserts simple string value at the position
            valueAfterChange = conv.ToString(); // Gets new value
            String addedVal_2 = conv.AddBinary("0011 1111"); // Adds binary value at the end
            String valueAfterChange_2 = conv.ToString(); // Gets new value

            Console.WriteLine("--------------------");
            Console.WriteLine("Value before change: " + valueBeforeChange);
            Console.WriteLine("Value before change(Hex): " + valueBeforeChangeHex);
            Console.WriteLine("Returned value: " + addedVal);
            Console.WriteLine("Value after change: " + valueAfterChange);
            Console.WriteLine("Returned value 2: " + addedVal_2);
            Console.WriteLine("Value after change 2: " + valueAfterChange_2);
            Console.WriteLine("--------------------");

        }
```
```
--------------------
Binary: 1111101
Octal: 175
Decimal: 125
Hex: 7d
Original: 125
Original Type: Int32

--------------------
Binary: 1 111 101
Octal: 175
Decimal: 125
Hex: 7d
Original: 125
Original Type: Int32

--------------------
Binary: 1-111-101
Octal: 175
Decimal: 125
Hex: 7d
Original: 125
Original Type: Int32

--------------------
--------------------
Object's value: 125
Binary List printed: [1, 1, 1, 1, 1, 0, 1]
Hex List printed: [7, d]
Octal List printed: [1, 7, 5]
Dec List printed: [1, 2, 5]
--------------------
--------------------
Value before change: 125
Value before change(Hex): 7d
Returned value: 7fdf
Value after change: 32735
--------------------
--------------------
Value before change: 32735
Value before change(Hex): 7fdf
Returned value: 3122735
Value after change: 3122735
Returned value 2: 101111101001100010111100111111
Value after change 2: 799420223
--------------------

```

<a name="example_2"></a>
#### Example with String

```c#
private static void ConverterExample_WithString()
        {
            Converter conv = new Converter(); // Create empty converter
            conv.SetValue("Example", Encoding.ASCII); // Set string value and different encoding

            String convFullData = conv.ToFullString(); // Gets object's value's all data as string
            String convFullDataWithSpaces = conv.ToFullString(3); // Gets object's value's all data as string and adds space between elemetns
            String convFullDataWithCharSpaces = conv.ToFullString(3, '-'); // Gets object's value's all data as string and adds char symbol between elements

            Console.WriteLine("--------------------");
            Console.WriteLine(convFullData);
            Console.WriteLine("--------------------");
            Console.WriteLine(convFullDataWithSpaces);
            Console.WriteLine("--------------------");
            Console.WriteLine(convFullDataWithCharSpaces);
            Console.WriteLine("--------------------");

            List<Char> binaryList = conv.ToBinaryArray(); // Return value as Binary value in List<Char> format
            List<Char> hexList = conv.ToHexArray(); // Return value as Hex value in List<Char> format
            List<Char> octalList = conv.ToOctalArray(); // Return value as Octal value in List<Char> format
            List<Char> decList = conv.ToDecArray(); // Return value as Decimal value in List<Char> format

            String savedValue = conv.ToString(); // Returns set value as string

            Console.WriteLine("--------------------");
            Console.WriteLine("Object's value: " + savedValue);
            Console.WriteLine("Binary List printed: [" + String.Join(", ", binaryList) + "]");
            Console.WriteLine("Hex List printed: [" + String.Join(", ", hexList) + "]");
            Console.WriteLine("Octal List printed: [" + String.Join(", ", octalList) + "]");
            Console.WriteLine("Dec List printed: [" + String.Join(", ", decList) + "]");
            Console.WriteLine("--------------------");


            String valueBeforeChange = conv.ToString(); // Gets current value
            String valueBeforeChangeHex = conv.ToHexString(); // Gets current value in hex format

            String replace = conv.ReplaceHex("7d", "44"); // Replaces Hex value's 65 with 44 making our Example to ExamplD
            String valueAfterChange = conv.ToString(); // Gets new value

            // Prints out values
            Console.WriteLine("--------------------");
            Console.WriteLine("Value before change: " + valueBeforeChange);
            Console.WriteLine("Value before change(Hex): " + valueBeforeChangeHex);
            Console.WriteLine("Returned value: " + replace);
            Console.WriteLine("Value after change: " + valueAfterChange);
            Console.WriteLine("--------------------");


            valueBeforeChange = conv.ToString(); // Gets current value
            valueBeforeChangeHex = conv.ToHexString();

            String addedVal = conv.AddVal(" Ad ", 1); // Inserts simple string value at the position
            valueAfterChange = conv.ToString(); // Gets new value
            String addedVal_2 = conv.AddBinary("0011 1111"); // Adds binary value at the end
            String valueAfterChange_2 = conv.ToString(); // Gets new value

            Console.WriteLine("--------------------");
            Console.WriteLine("Value before change: " + valueBeforeChange);
            Console.WriteLine("Value before change(Hex): " + valueBeforeChangeHex);
            Console.WriteLine("Returned value: " + addedVal);
            Console.WriteLine("Value after change: " + valueAfterChange);
            Console.WriteLine("Returned value 2: " + addedVal_2);
            Console.WriteLine("Value after change 2: " + valueAfterChange_2);
            Console.WriteLine("--------------------");

        }
```
```
--------------------
Binary: 01000101011110000110000101101101011100000110110001100101
Octal: 105170141155160154145
Decimal: 6912097109112108101
Hex: 4578616d706c65
Original: Example
Original Type: String

--------------------
Binary: 01 000 101 011 110 000 110 000 101 101 101 011 100 000 110 110 001 100 101
Octal: 105 170 141 155 160 154 145
Decimal: 6 912 097 109 112 108 101
Hex: 45 786 16d 706 c65
Original: Example
Original Type: String

--------------------
Binary: 01-000-101-011-110-000-110-000-101-101-101-011-100-000-110-110-001-100-101
Octal: 105-170-141-155-160-154-145
Decimal: 6-912-097-109-112-108-101
Hex: 45-786-16d-706-c65
Original: Example
Original Type: String

--------------------
--------------------
Object's value: Example
Binary List printed: [0, 1, 0, 0, 0, 1, 0, 1, 0, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 0, 1, 1, 0, 1, 1, 0, 1, 0, 1, 1, 1, 0, 0, 0, 0, 0, 1, 1, 0, 1, 1, 0, 0, 0, 1, 1, 0, 0, 1, 0, 1]
Hex List printed: [4, 5, 7, 8, 6, 1, 6, d, 7, 0, 6, c, 6, 5]
Octal List printed: [1, 0, 5, 1, 7, 0, 1, 4, 1, 1, 5, 5, 1, 6, 0, 1, 5, 4, 1, 4, 5]
Dec List printed: [6, 9, 1, 2, 0, 9, 7, 1, 0, 9, 1, 1, 2, 1, 0, 8, 1, 0, 1]
--------------------
--------------------
Value before change: Example
Value before change(Hex): 4578616d706c65
Returned value: 4578616d706c65
Value after change: Example
--------------------
--------------------
Value before change: Example
Value before change(Hex): 4578616d706c65
Returned value: E Ad xample
Value after change: E Ad xample
Returned value 2: 010001010010000001000001011001000010000001111000011000010110110101110000011011000110010100111111
Value after change 2: E Ad xample?
--------------------

```

<a name="example_3"></a>
### TypeConverter Example code
```c#
private static void TypeConverterExample()
        {
            TypeConverter converter = new TypeConverter();

            String binary = "1010";
            String hex = "F6D4";
            String octal = "1254";
            long decimalVal = 1234;

            // Converts binary to hex, octal, dec types
            String binToHex = converter.BinaryToHex(binary);
            String binToOctal = converter.BinaryToOctal(binary);
            String binToDec = converter.BinaryToDec(binary);

            // Converts hex to binary, octal, dec types
            String hexToBinary = converter.HexToBinary(hex);
            String hexToOctal = converter.HexToOctal(hex);
            String hexToDec = converter.HexToDec(hex);

            // Converts octal to hex, binary, dec types
            String octalToBinary = converter.OctalToBinary(octal);
            String octalToDec = converter.OctalToDec(octal);
            String octalToHex = converter.OctalToHex(octal);

            // Converts dec to hex, octal, binary types
            String decToBinary = converter.DecToBinary(decimalVal);
            String decToHex = converter.DecToHex(decimalVal);
            String decToOctal = converter.DecToOctal(decimalVal);

            // Prints out all converted values to console
            Console.WriteLine("|---Binary---|");
            Console.WriteLine("Orginal -> " + binary);
            Console.WriteLine("Converted to Hex -> " + binToHex);
            Console.WriteLine("Converted to Octal -> " + binToOctal);
            Console.WriteLine("Converted to Decimal -> " + binToDec);

            Console.WriteLine();

            Console.WriteLine("|---Hex---|");
            Console.WriteLine("Orginal -> " + hex);
            Console.WriteLine("Converted to Binary -> " + hexToBinary);
            Console.WriteLine("Converted to Octal -> " + hexToOctal);
            Console.WriteLine("Converted to Decimal -> " + hexToDec);

            Console.WriteLine();

            Console.WriteLine("|---Octal---|");
            Console.WriteLine("Orginal -> " + octal);
            Console.WriteLine("Converted to Binary -> " + octalToBinary);
            Console.WriteLine("Converted to Dec -> " + octalToDec);
            Console.WriteLine("Converted to Hex -> " + octalToHex);

            Console.WriteLine();

            Console.WriteLine("|---Decimal---|");
            Console.WriteLine("Orginal -> " + decimalVal.ToString());
            Console.WriteLine("Converted to Binary -> " + decToBinary);
            Console.WriteLine("Converted to Hex -> " + decToHex);
            Console.WriteLine("Converted to Octal -> " + decToOctal);
        }
```

### Output

```c#
|---Binary---|
Orginal -> 1010
Converted to Hex -> 0A
Converted to Octal -> 12
Converted to Decimal -> 10

|---Hex---|
Orginal -> F6D4
Converted to Binary -> 1111011011010100
Converted to Octal -> 173 324
Converted to Decimal -> 63188

|---Octal---|
Orginal -> 1254
Converted to Binary -> 001010101100
Converted to Dec -> 684
Converted to Hex -> 02 AC

|---Decimal---|
Orginal -> 1234
Converted to Binary -> 10011010010
Converted to Hex -> 4D2
Converted to Octal -> 2322
```
