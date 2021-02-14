

# Class SPCT.TypeConverter

## Description:

Class [TypeConverter](TypeConverter.md)

Class which provides the user to perform conversion of different types.

Conversion is possible from and to these types: binary, hex, octal, decimal.

**Warning:** Methods are not set up to test if provided values are in correct format, when an overflow happens when converting from one type to another is also not controlled.

## Provided methods:
| Modifier | Method | Description |
|-|-|-|
|**public**|String [HexToBinary](#HexToBinary)(String value)|Converts provided Hex String to Binary|
|**public**|String [HexToDec](#HexToDec)(String value)|Converts provided Hex String to Dec|
|**public**|String [HexToOctal](#HexToOctal)(String value)|Converts provided Hex String to Octal|
|**public**|String [BinaryToOctal](#BinaryToOctal)(String value)|Converts provided Binary String to Octal|
|**public**|String [BinaryToDec](#BinaryToDec)(String value)|Converts provided Binary String to Dec|
|**public**|String [BinaryToHex](#BinaryToHex)(String value)|Converts provided Binary String to Hex|
|**public**|String [DecToBinary](#DecToBinary)(Int64 value)|Converts provided Dec String to Binary|
|**public**|String [DecToOctal](#DecToOctal)(Int64 value)|Converts provided Dec String to Octal|
|**public**|String [DecToHex](#DecToHex)(Int64 value)|Converts provided Dec String to Hex|
|**public**|String [OctalToBinary](#OctalToBinary)(String value)|Converts provided Octal String to Binary|
|**public**|String [OctalToDec](#OctalToDec)(String value)|Converts provided Octal String to Dec|
|**public**|String [OctalToHex](#OctalToHex)(String value)|Converts provided Octal String to Hex|
|**public**|String [RemoveLeadingZeros](#RemoveLeadingZeros)(String value)|Removes all leading leading zeros|
|**public**|String [RemoveAllAdditionalSymbols](#RemoveAllAdditionalSymbols)(String val)|Removes all special symbols from specified string|



## Constructors and methods details:

<a name="BinaryToDec"></a>

```c#
 public string BinaryToDec(string value)
```

* Converts provided Binary String to Dec

**Parameters:**

* String value - Binary String value

**Returns:**

* String of Dec value
---

<a name="BinaryToHex"></a>
```c#
public string BinaryToHex(string value)
```
* Converts provided Binary String to Hex

**Parameters:**

* String value - Binary String value

**Returns:**

* String of Hex value
---

<a name="BinaryToOctal"></a>
```c#
public string BinaryToOctal(string value)
```

* Converts provided Binary String to Octal

**Parameters:**

* String value - Binary String value

**Returns:**

* String of Octal value
---

<a name="DecToBinary"></a>
```c#
public string DecToBinary(long value)
```

* Converts provided Dec String to Binary

**Parameters:**

* Long value - Dec String value

**Returns:**

* String of Binary value

---
<a name="DecToHex"></a>
```c#
public string DecToHex(long value)
```

* Converts provided Dec String to Hex

**Parameters:**

* Long value - Dec String value

**Returns:**

* String of Hex value

---
<a name="DecToOctal"></a>
```c#
public string DecToOctal(long value)
```

* Converts provided Dec String to Octal

**Parameters:**

* Long value - Dec String value

**Returns:**

* String of Octal value

---
<a name="HexToBinary"></a>
```c#
public string HexToBinary(string value)
```

* Converts provided Hex String to Binary

**Parameters:**

* String value - Hex String value

**Returns:**

* String of binary value

---
<a name="HexToDec"></a>
```c#
public string HexToDec(string value)
```

* Converts provided Hex String to Dec

**Parameters:**

* String value - Hex String value

**Returns:**

* String of Dec value

---
<a name="HexToOctal"></a>
```c#
public string HexToOctal(string value)
```

* Converts provided Hex String to Octal

**Parameters:**

* String value - Hex String value

**Returns:**

* String of Octal value

---
<a name="OctalToBinary"></a>
```c#
public string OctalToBinary(string value)
```

* Converts provided Octal String to Binary

**Parameters:**

* String value - Octal String value

**Returns:**

* String of Binary value

---
<a name="OctalToDec"></a>
```c#
public string OctalToDec(string value)
```

* Converts provided Octal String to Dec

**Parameters:**

* String value - Octal String value

**Returns:**

* String of Dec value

---
<a name="OctalToHex"></a>
```c#
public string OctalToHex(string value)
```

* Converts provided Octal String to Hex

**Parameters:**

* String value - Octal String value

**Returns:**

* String of Hex value

---
<a name="RemoveAllAdditionalSymbols"></a>
```c#
public string RemoveAllAdditionalSymbols(string val)
```

* Removes all special symbols from specified string

**Parameters:**

* String val - String to modify

**Returns:**

* Modified string

---
<a name="RemoveLeadingZeros"></a>
```c#
public string RemoveLeadingZeros(string value)
```

* Removes all leading leading zeros

**Parameters:**

* String value - String value to remove from

**Returns:**

* Modified string value

---
