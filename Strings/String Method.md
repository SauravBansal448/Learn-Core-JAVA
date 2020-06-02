# String Method 

* **int length():** Returns the number of characters in the String.

```
"Mobcoder LLC".length(); returns 12
```

* **Char charAt(int i):** Returns the character at ith index.

```
"Mobcoder LLC".charAt(3); returns c
```

* **String substring (int i):** Return the substring from the ith  index character to end.

```
"Mobcoder LLC".substring(8); returns LLC
```

* **String substring (int i, int j):** Returns the substring from i to j-1 index.

```
"Mobcoder LLC".substring(3,7); returns ode
```

* **String concat( String str):** Concatenates specified string to the end of this string.

```
 String s1 = ”Mobcoder”;
 String s2 = ” LLC”;
 String output = s1.concat(s2); // returns “Mobcoder LLC”
```

* **int indexOf (String s):** Returns the index within the string of the first occurrence of the specified string.

```
 String s = ”Mobcoder LLC”;
 int output = s.indexOf(“LLC”); // returns 9
```

* **int indexOf (String s, int i):** Returns the index within the string of the first occurrence of the specified string, starting at the specified index.

```
String s = "Mobcoder LLC";
int output = s.indexOf("od",2);   //return 4
```

* **Int lastIndexOf( String s):** Returns the index within the string of the last occurrence of the specified string.\

```
 String s = ”Mobcoder LLC”;
 int output = s.lastIndexOf("o"); // returns 4
```

* **boolean equals( Object otherObj):** Compares this string to the specified object.

```
 Boolean out = “Mobcoder”.equals(“Mobcoder”); // returns true
 Boolean out = “Mobcoder”.equals(“MOBCODER”); // returns false
```

* **boolean  equalsIgnoreCase (String anotherString):** Compares string to another string, ignoring case considerations.

```
 Boolean out = “Mobcoder”.equalsIgnoreCase(“Mobcoder”); // returns true
 Boolean out = “Mobcoder”.equalsIgnoreCase(“MOBCODER”); // returns true
```
* **String toLowerCase():** Converts all the characters in the String to lower case.

```
String word1 = “Mobcoder LLC”;
String word3 = word1.toLowerCase(); // returns “mobcoder llc"
```

* **String toUpperCase():** Converts all the characters in the String to upper case.

```
String word1 = “Mobcoder LLC”;
String word3 = word1.toUpperCase(); // returns “MOBCODER LLC"
```

* **String trim():** Returns the copy of the String, by removing whitespaces at both ends. It does not affect whitespaces in the middle.

```
String word1 = “ Mobcoder LLC “;
String word2 = word1.trim(); // returns “Mobcoder LLC”
```

*  **String replace (char oldChar, char newChar):** Returns new string by replacing all occurrences of oldChar with newChar.

```
String s1 = “Mobcoder LLP“;
String s2 = “Mobcoder LLP”.replace(‘P’ ,’C’); // returns “Mobcoder LLC”
```

* **int compareTo( String anotherString):** Compares two string lexicographically.

```
 int out = s1.compareTo(s2);  // where s1 ans s2 are
                             // strings to be compared

 This returns difference s1-s2. If :
 out < 0  // s1 comes before s2
 out = 0  // s1 and s2 are equal.
 out > 0   // s1 comes after s2.
 
```

* **int compareToIgnoreCase( String anotherString):** Compares two string lexicographically, ignoring case considerations.

```
 int out = s1.compareToIgnoreCase(s2);  // where s1 ans s2 are 
                                        // strings to be compared

 This returns difference s1-s2. If :
 out < 0  // s1 comes before s2
 out = 0   // s1 and s2 are equal.
 out > 0   // s1 comes after s2.
```
