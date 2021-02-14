
# Class SPCT.Converter

## Inherited classes:

Class [SPCT.TypeConverter](TypeConverter.md)

## Description:

**Class [Converter](Converter.md): [TypeConverter](TypeConverter.md)**

* Class which provides user a way to set a value through a constructor or through a method.
* Provided value can be in either Int16, Int32, Int64 or String type.
* Once the object is created user can perform conversions, receive the value, and make changes to it.
* Conversion is possible from and to these types: binary, hex, octal, decimal.

**Warning:** Methods are not set up to test if provided values are in correct format, when an overflow happens when converting from one type to another is also not controlled.

## Constructors:

|**Modifier**|**Constructor**|**Description**|
|-|-|-
|**public**|[Converter](#Converter1)()|Constructs a new Converter object with no value set – empty constructor|
|**public**|[Converter](#Converter2)(string value)|Constructs a new Converter object with new string value and default UTF32 encoding|
|**public**|[Converter](#Converter3)(short value)|Constructs a new Converter object with new short value|
|**public**|[Converter](#Converter4)(int value)|Constructs a new Converter object with new int value|
|**public**|[Converter](#Converter5)(long value)|Constructs a new Converter object with new long value|
|**public**|[Converter](#Converter6)(string value, Encoding encoding)|Constructs a new Converter object with new string value and specified encoding|

## Provided methods:

| Modifier | Method | Description |
|-|-|-|
|**public**|string [AddBinary](#AddBinary1)(string value, int from)|Adds provided value to object's value's string. Insert is performed from provided location. Performed on Binary type level.|
|**public**|string [AddBinary](#AddBinary2)(string value)|Adds provided value to object's value's string. Insert is performed from provided location. Performed on Binary type level.|
|**public**|string [AddDec](#AddDec1)(string value, int from)|Adds provided value to object's value's string. Insert is performed from provided location. Performed on Dec type level.|
|**public**|string [AddDec](#AddDec2)(string value)|Adds provided value to object's value's string. Performed on Dec type level.|
|**public**|string [AddHex](#AddHex1)(string value, int from)|Adds provided value to object's value's string. Insert is performed from provided location. Performed on Hex type level.|
|**public**|string [AddHex](#AddHex2)(string value)|Adds provided value to object's value's string. Performed on Hex type level.|
|**public**|string [AddOctal](#AddOctal1)(string value, int from)|Adds provided value to object's value's string. Insert is performed from provided location. Performed on Octal type level.|
|**public**|string [AddOctal](#AddOctal2)(string value)|Adds provided value to object's value's string. Performed on Octal type level.|
|**public**|string [AddVal](#AddVal1)(string value)|Adds provided value to object's value's string.|
|**public**|string [AddVal](#AddVal2)(string value, int from)|Adds provided value to object's value's string. Insert is performed from provided location.|
|**public**|string [BinaryToString](#BinaryToString1)(List<byte> binary)|Converts provided binary array to string.|
|**public**|string [ClassToString](#ClassToString1)|Returns the Class name of saved object.|
|**public**|string [ReplaceBinary](#ReplaceBinary1)(string from, string to)|Replaces saved value from to where replacement is performed on binary value. The new value is returned and set.|
|**public**|string [ReplaceDec](#ReplaceDec1)(string from, string to)|Replaces saved value from to where replacement is performed on Dec value. The new value is returned and set.|
|**public**|string [ReplaceHex](#ReplaceHex1)(string from, string to)|Replaces saved value from to where replacement is performed on hex value. The new value is returned and set.|
|**public**|string [ReplaceOctal](#ReplaceOctal1)(string from, string to)|Replaces saved value from to where replacement is performed on Octal value. The new value is returned and set.|
|**public**|string [ReplaceVal](#ReplaceVal)(string from, string to)|Replaces saved value from to. The new value is returned and set.|
|**public**|void [SetCurrentValue](#SetCurrentValue1)(string value)|Set current object's value using provided string value.|
|**public**|void [SetValue](#SetValue1)(string value)|Method used to (re)set the value.|
|**public**|void [SetValue](#SetValue2)(string value, Encoding encoding)|Method used to (re)set the value.|
|**public**|void [SetValue](#SetValue3)(short value)|Method used to (re)set the value.|
|**public**|void [SetValue](#SetValue4)(int value)|Method used to (re)set the value.|
|**public**|void [SetValue](#SetValue5)(long value)|Method used to (re)set the value.|
|**public**|List<char> [ToBinaryArray](#ToBinaryArray1)()|Returns value's binary value as Char List.|
|**public**|string [ToBinaryString](#ToBinaryString1)()|Method used to return current value as binary string.|
|**public**|string [ToBinaryString](#ToBinaryString2)(int spaces)|Method used to return current value as binary string Also add spaces between specified amounts of elements.|
|**public**|string [ToBinaryString](#ToBinaryString3)(int spaces, char seperator)|Method used to return current value as binary string. Also add spaces between specified amounts of elements. Also specified char symbol is going to be placed in added space.|
|**public**|List<char> [ToDecArray](#ToDecArray1)()|Returns value's dec value as Char List.|
|**public**|string [ToDecString](#ToDecString1)(int spaces, char seperator)|Method used to return current value as dec string. Also add spaces between specified amounts of elements. Also specified char symbol is going to be placed in added space.|
|**public**|string [ToDecString](#ToDecString2)()|Method used to return current value as dec string.|
|**public**|string [ToDecString](#ToDecString3)(int spaces)|Method used to return current value as dec string. Also add spaces between specified amounts of elements.|
|**public**|string [ToFullString](#ToFullString1)()|Used to print saved value in all formats: binary, string, octal, dec, original, class name.|
|**public**|string [ToFullString](#ToFullString2)(int spaces, char seperator)|Used to print saved value in all formats: binary, string, octal, dec, original, class name. Also add spaces between values. Also specifed the symbol that will be added in space.|
|**public**|string [ToFullString](#ToFullString3)(int spaces)|Used to print saved value in all formats: binary, string, octal, dec, original, class name. Also add spaces between values.|
|**public**|List<char> [ToHexArray](#ToHexArray1)()|Returns value's hex value as Char List.|
|**public**|string [ToHexString](#ToHexString1)(int spaces, char seperator)|Method used to return current value as hex string. Also add spaces between specified amounts of elements. Also specified char symbol is going to be placed in added space.|
|**public**|string [ToHexString](#ToHexString2)(int spaces)|Method used to return current value as hex string. Also add spaces between specified amounts of elements.|
|**public**|string [ToHexString](#ToHexString3)()|Method used to return current value as hex string.|
|**public**|List<char> [ToOctalArray](#ToOctalArray1)()|Returns value's hex value as Char List.|
|**public**|string [ToOctalString](#ToOctalString1)()|Method used to return current value as octal string.|
|**public**|string [ToOctalString](#ToOctalString2)(int spaces)|Method used to return current value as octal string. Also add spaces between specified amounts of elements.|
|**public**|string [ToOctalString](#ToOctalString3)(int spaces, char seperator)|Method used to return current value as octal string. Also add spaces between specified amounts of elements. Also specified char symbol is going to be placed in added space.|
|**public**|override string [ToString](#ToString1)()|Method used to return current saved value as string.|

## Inherited methods:

**Methods From TypeConverter.cs**

| Modifier | Method | Description |
|-|-|-|
|**public**|String [HexToBinary](TypeConverter.md/#HexToBinary)(String value)|Converts provided Hex String to Binary|
|**public**|String [HexToDec](TypeConverter.md/#HexToDec)(String value)|Converts provided Hex String to Dec|
|**public**|String [HexToOctal](TypeConverter.md/#HexToOctal)(String value)|Converts provided Hex String to Octal|
|**public**|String [BinaryToOctal](TypeConverter.md/#BinaryToOctal)(String value)|Converts provided Binary String to Octal|
|**public**|String [BinaryToDec](TypeConverter.md/#BinaryToDec)(String value)|Converts provided Binary String to Dec|
|**public**|String [BinaryToHex](TypeConverter.md/#BinaryToHex)(String value)|Converts provided Binary String to Hex|
|**public**|String [DecToBinary](TypeConverter.md/#DecToBinary)(Int64 value)|Converts provided Dec String to Binary|
|**public**|String [DecToOctal](TypeConverter.md/#DecToOctal)(Int64 value)|Converts provided Dec String to Octal|
|**public**|String [DecToHex](TypeConverter.md/#DecToHex)(Int64 value)|Converts provided Dec String to Hex|
|**public**|String [OctalToBinary](TypeConverter.md/#OctalToBinary)(String value)|Converts provided Octal String to Binary|
|**public**|String [OctalToDec](TypeConverter.md/#OctalToDec)(String value)|Converts provided Octal String to Dec|
|**public**|String [OctalToHex](TypeConverter.md/#OctalToHex)(String value)|Converts provided Octal String to Hex|
|**public**|String [RemoveLeadingZeros](TypeConverter.md/#RemoveLeadingZeros)(String value)|Removes all leading leading zeros|
|**public**|String [RemoveAllAdditionalSymbols](TypeConverter.md/#RemoveAllAdditionalSymbols)(String val)|Removes all special symbols from specified string|


## Constructors and methods details:

<a name="Converter1"></a>
```c#
public Converter()
```
* Constructs a new Converter object with no value set – empty constructor

---
<a name="Converter2"></a>
```c#
public Converter(string value)
```

* Constructs a new Converter object with new string value and default UTF32 encoding

**Parameters:**

* String value - value which will be used for modifications and conversion in class

---
<a name="Converter3"></a>
```c#
public Converter(short value)
```

* Constructs a new Converter object with new short value

**Parameters:**

* Int16 value - Int16 Value used for further modifications

---
<a name="Converter4"></a>
```c#
public Converter(int value)
```

* Constructs a new Converter object with new int value

**Parameters:**

* Int32 value - Int32 Value used for further modifications

---
<a name="Converter5"></a>
```c#
public Converter(long value)
```

* Constructs a new Converter object with new long value

**Parameters:**

* Int64 value - Int64 Value used for further modifications

---
<a name="Converter6"></a>
```c#
public Converter(string value, Encoding encoding)
```

* Constructs a new Converter object with new string value and specified encoding

**Parameters:**

* String value - String value, which will be used for modifications

* Encoding encoding - Encoding type for conversions

---
<a name="AddBinary1"></a>
```c#
public string AddBinary(string value, int from)
```

* Adds binary string to object’s value in binary format level

**Parameters:**

* String value – value to insert into object’s string

* Int from – location to insert from

**Returns:**

* String – newly modified binary string value

---
<a name="AddBinary2"></a>
```c#
public string AddBinary(string value)
```

* Adds provided value to object's value's string. Performed on Binary type level.

**Parameters:**

* String value – value to insert into object’s string

**Returns:**

* Returns newly set value

---
<a name="AddDec1"></a>
```c#
public string AddDec(string value, int from)
```

* Adds provided value to object's value's string. Insert is performed from provided location. Performed on Dec type level.

**Parameters:**

* String value – Value to add

* Int from - Adds value from specified location

**Returns:**

* Returns newly set value.

---
<a name="AddDec2"></a>
```c# 
public string AddDec(string value) 
```

* Adds provided value to object's value's string. Performed on Dec type level.

**Parameters:**

* String value – Value to add

**Returns:**

* Returns newly set value

---
<a name="AddHex1"></a>
```c# 
public string AddHex(string value, int from) 
```

* Adds provided value to object's value's string. Insert is performed from provided location. Performed on Hex type level.

**Parameters:**

* String value – Value to add

* Int from - Adds value from specified location

**Returns:**

* Returns newly set value

---
<a name="AddHex2"></a>
```c# 
public string AddHex(string value) 
```

* Adds provided value to object's value's string. Performed on Hex type level.

**Parameters:**

* String value – Value to add

**Returns:**

* Returns newly set value

---
<a name="AddOctal1"></a>
```c# 
public string AddOctal(string value, int from) 
```

* Adds provided value to object's value's string. Insert is performed from provided location. Performed on Octal type level.

**Parameters:**

* String value – Value to add

* Int from - Adds value from specified location

**Returns:**

* Returns newly set value

---
<a name="AddOctal2"></a>
```c# 
public string AddOctal(string value) 
```

* Adds provided value to object's value's string. Performed on Octal type level.

**Parameters:**

* String value – Value to add

**Returns:**

* Returns newly set value

---
<a name="AddVal1"></a>
```c# 
public string AddVal(string value) 
```

* Adds provided value to object's value's string.

**Parameters:**

* String value – Value to add

**Returns:**

* Returns newly set value

---
<a name="AddVal2"></a>
```c# 
public string AddVal(string value, int from) 
```

* Adds provided value to object's value's string. Insert is performed from provided location.

**Parameters:**

* String value – Value to add

**Returns:**

* Returns newly set value

---
<a name="BinaryToString1"></a>
```c# 
public string BinaryToString(List<byte> binary) 
```

* Converts provided binary array to string

**Parameters:**

* List<byte> value – list of binary bytes

**Returns:**

* Binary string

---
<a name="ClassToString1"></a>
```c# 
public string ClassToString() 
```

* Returns the Class name of saved object

**Returns:**

* Returns Class name as string

---
<a name="ReplaceBinary1"></a>
```c# 
public string ReplaceBinary(string from, string to) 
```

* Replaces saved value from to where replacement is performed on binary value. The new value is returned and set.

**Parameters:**

* String from – String to replace from

* String to – String to replace to

**Returns:**

* Changed Binary value

---
<a name="ReplaceDec1"></a>
```c# 
public string ReplaceDec(string from, string to) 
```

* Replaces saved value from to where replacement is performed on Dec value. The new value is returned and set.

**Parameters:**

* String from – String to replace from

* String to – String to replace to

**Returns:**

* Changed Dec value

---
<a name="ReplaceHex1"></a>
```c# 
public string ReplaceHex(string from, string to) 
```

* Replaces saved value from to where replacement is performed on hex value. The new value is returned and set.

**Parameters:**

* String from – String to replace from

* String to – String to replace to

**Returns:**

* Changed Hex value

---
<a name="ReplaceOctal1"></a>
```c# 
public string ReplaceOctal(string from, string to) 
```

* Replaces saved value from to where replacement is performed on Octal value. The new value is returned and set.

**Parameters:**

* String from – String to replace from

* String to – String to replace to

**Returns:**

* Changed Octal value

---
<a name="ReplaceVal1"></a>
```c# 
public string ReplaceVal(string from, string to) 
```

* Replaces saved value from to The new value is returned and set.

**Parameters:**

* String from – String to replace from

* String to – String to replace to

**Returns:**

* Changed value

---
<a name="SetCurrentValue1"></a>
```c# 
public void SetCurrentValue(string value) 
```

* Set current object's value using provided string value

**Parameters:**

* String value - String value, which will be set

---
<a name="SetValue1"></a>
```c# 
public void SetValue(string value) 
```

* Method used to (re)set the value

**Parameters:**

* String value – String value to be set

---
<a name="SetValue2"></a>
```c# 
public void SetValue(string value, Encoding encoding) 
```

* Method used to (re)set the value

**Parameters:**

* String value – String value to be set

* Encoding encoding - Encoding type to be set

---
<a name="SetValue3"></a>
```c# 
public void SetValue(short value) 
```

* Method used to (re)set the value

**Parameters:**

* Short value – Int16 value to be set

---
<a name="SetValue4"></a>
```c# 
public void SetValue(int value) 
```

* Method used to (re)set the value

**Parameters:**

* Int32 value – Int32 value to be set

---
<a name="SetValue5"></a>
```c# 
public void SetValue(long value) 
```

* Method used to (re)set the value

**Parameters:**

* Int64 value – Int64 value to be set

---
<a name="ToBinaryArray1"></a>
```c# 
public List<char> ToBinaryArray() 
```

* Returns value's binary value as Char List.

**Returns:**

* Char list of binary.

---
<a name="ToBinaryString1"></a>
```c# 
public string ToBinaryString() 
```

* Method used to return current value as binary string.

**Returns:**

* Returns binary value as string of current set value.

---
<a name="ToBinaryString2"></a>
```c# 
public string ToBinaryString(int spaces) 
```

* Method used to return current value as binary string. Also add spaces between specified amounts of elements.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

**Returns:**

* Returns binary value as string of current set value.

---
<a name="ToBinaryString3"></a>
```c# 
public string ToBinaryString(int spaces, char seperator) 
```

* Method used to return current value as binary string. Also add spaces between specified amounts of elements. Also specified char symbol is going to be placed in added space.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

* Char separator - The char symbol which will be placed in added space

**Returns:**

* Returns binary value as string of current set value.

---
<a name="ToDecArray1"></a>
```c# 
public List<char> ToDecArray() 
```

* Returns value's dec value as Char List.

**Returns:**

* Char list of dec.

---
<a name="ToDecString1"></a>
```c# 
public string ToDecString(int spaces, char seperator) 
```

* Method used to return current value as dec string. Also add spaces between specified amounts of elements. Also specified char symbol is going to be placed in added space.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

* Char separator - The char symbol which will be placed in added space

**Returns:**

* Returns dec value as string of current set value.

---
<a name="ToDecString2"></a>
```c# 
public string ToDecString() 
```

* Method used to return current value as dec string.

**Returns:**

* Returns dec value as string of current set value.

---
<a name="ToDecString3"></a>
```c# 
public string ToDecString(int spaces) 
```

* Method used to return current value as dec string. Also add spaces between specified amounts of elements.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

**Returns:**

* Returns dec value as string of current set value.

---
<a name="ToFullString1"></a>
```c# 
public string ToFullString() 
```

* Used to print saved value in all formats: binary, string, octal, dec, original, class name.

**Returns:**

* Multi-line string value of information about the value.

---
<a name="ToFullString2"></a>
```c# 
public string ToFullString(int spaces, char seperator) 
```

* Used to print saved value in all formats: binary, string, octal, dec, original, class name. Also add spaces between values. Also specified the symbol that will be added in space.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

* Char separator - The char symbol which will be placed in added space

**Returns:**

* Multi-line string value of information about the value.

---
<a name="ToFullString3"></a>
```c# 
public string ToFullString(int spaces) 
```

* Used to print saved value in all formats: binary, string, octal, dec, original, class name. Also add spaces between values.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

**Returns:**

* Multi-line string value of information about the value.

---
<a name="ToHexArray1"></a>
```c# 
public List<char> ToHexArray() 
```

* Returns value's hex value as Char List.

**Returns:**

* Char list of hex.

---
<a name="ToHexString1"></a>
```c# 
public string ToHexString(int spaces, char seperator) 
```

* Method used to return current value as hex string. Also add spaces between specified amounts of elements. Also specified char symbol is going to be placed in added space.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

* Char separator - The char symbol which will be placed in added space

**Returns:**

* Returns hex value as string of current set value.

---
<a name="ToHexString2"></a>
```c# 
public string ToHexString(int spaces) 
```

* Method used to return current value as hex string. Also add spaces between specified amounts of elements.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

**Returns:**

* Returns hex value as string of current set value.

---
<a name="ToHexString3"></a>
```c# 
public string ToHexString() 
```

* Method used to return current value as hex string.

**Returns:**

* Returns hex value as string of current set value.

---
<a name="ToOctalArray1"></a>
```c# 
public List<char> ToOctalArray() 
```

* Returns value's octal value as Char List.

**Returns:**

* Char list of octal.

---
<a name="ToOctalString1"></a>
```c# 
public string ToOctalString() 
```

* Method used to return current value as octal string.

**Returns:**

* Returns octal value as string of current set value.

---
<a name="ToOctalString2"></a>
```c# 
public string ToOctalString(int spaces) 
```

* Method used to return current value as octal string. Also add spaces between specified amounts of elements.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

**Returns:**

* Returns octal value as string of current set value.

---
<a name="ToOctalString3"></a>
```c# 
public string ToOctalString(int spaces, char seperator) 
```

* Method used to return current value as octal string. Also add spaces between specified amounts of elements. Also specified char symbol is going to be placed in added space.

**Parameters:**

* Int spaces – Between how many elements the space is going to be added

* Char separator - The char symbol which will be placed in added space

**Returns:**

* Returns octal value as string of current set value.

---
<a name="ToString1"></a>
```c#
public override string ToString()
 ```

* Method used to return current saved value as string.

**Returns:**

* Returns saved value in string format.

---
