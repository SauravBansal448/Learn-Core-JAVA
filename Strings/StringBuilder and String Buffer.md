# StringBuilder and String Buffer

## String Buffer

- It reserves room for 16 characters without reallocation.
- StringBuffer represents growable and writable character sequences.
- All Implemented Interfaces of StringBuffer class: Serializable, Appendable, CharSequence.
- String buffers are safe for use by multiple threads. 

```
StringBuffer s=new StringBuffer();


StringBuffer s=new StringBuffer(20); // It accepts an integer argument that explicitly sets the size of the buffer.


StringBuffer s=new StringBuffer("Hello");
```

## String Builder

- String Builder is almost same as String Buffer but there is a diffrences between both which is:

* **StringBuilder is faster and preferred over StringBuffer for single threaded program.**
* **If thread safety is needed, then StringBuffer is used.**

```
StringBuilder s=new StringBuilder();


StringBuilder s=new StringBuilder(20);


StringBuilder s=new StringBuilder("Hello");
```

#### Note:
- objects of StringBuffer and StringBuilder are mutable
