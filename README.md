# CP11
## 12/6/2021

Binary Input/Output

File Abstraction
_Lowest level: Sequence of bytes
+Refer this as a stream
_How we interpret each byte (or group of bytes) depends on the context

Data types
Different primitive data types in Java require different amounts of space:
_byte: 1 byte
_short: 2 bytes
_int/float: 4 bytes
_double: 8 bytes

I/O Classes
Object
InputStream
_FileOutputStream, FilterOutputStream, ObjectInputStream
+DataoutputStream, BufferedInputStream
Character-Level Interaction
BufferedReader/BufferedWriter: Read/write individual character or entire Strings

Bufferings
_Storage devices store data in blocks of bytes
_Often more efficient to read/write entire blocks than the equivalent size a few bytes at a time
_BufferedReader reads an entire block at once and stores data temporarily in memory
_BufferedWriter stores written data temporarily in memory and then writes the data when a block is complete

Data-Level Interation
_Want to store primitive types in the file without having o deal directly at the byte level
+DataInputStream/DataoutputStream
+readShort(). readLong(), readDouble()
+writeShort(), writeLong(), writeDouble()
_Your program must keep track of the sequence that these primitive values are stored in

DataInputStream/DataOutputStream
Write/read Java primitives values and strings

Object-Level Interation
ObjectInputStream/ObjectOutputStream
_Can read/write entire objects in one call
_Read/write is recursive
+If an object contains references to other objects – they are read/written, too

## 8/12/21
Exam questions
