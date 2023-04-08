# Java_StringBuilder
StringBuilder in Java represents a mutable sequence of characters. Since the String Class in Java creates an immutable sequence of characters, the StringBuilder class provides an alternative to String Class, as it creates a mutable sequence of characters. The function of StringBuilder is very much similar to the StringBuffer class, as both of them provide an alternative to String Class by making a mutable sequence of characters. However, the StringBuilder class differs from the StringBuffer class on the basis of synchronization. The StringBuilder class provides no guarantee of synchronization whereas the StringBuffer class does. Therefore this class is designed for use as a drop-in replacement for StringBuffer in places where the StringBuffer was being used by a single thread (as is generally the case). Where possible, it is recommended that this class be used in preference to StringBuffer as it will be faster under most implementations. Instances of StringBuilder are not safe for use by multiple threads. If such synchronization is required then it is recommended that StringBuffer be used. String Builder is not thread-safe and high in performance compared to String buffer.
The class hierarchy is as follows:  ![Capture](https://user-images.githubusercontent.com/99464989/230713854-ef1f260a-5fc2-410b-8db2-283b51339610.PNG)
Constructors in Java StringBuilder Class 
StringBuilder(): Constructs a string builder with no characters in it and an initial capacity of 16 characters.
StringBuilder(int capacity): Constructs a string builder with no characters in it and an initial capacity specified by the capacity argument.
StringBuilder(CharSequence seq): Constructs a string builder that contains the same characters as the specified CharSequence.
StringBuilder(String str): Constructs a string builder initialized to the contents of the specified string. 
Below is a sample program to illustrate StringBuilder in Java. 
![Capture](https://user-images.githubusercontent.com/99464989/230713913-b8a842fe-8d31-4799-8fd6-3f7824a49e49.PNG)
![Capture](https://user-images.githubusercontent.com/99464989/230713930-2741a24d-afc0-4824-80b5-fb3d8a2c6de5.PNG)


                        

StringBuilder append(X x): This method appends the string representation of the X type argument to the sequence.
StringBuilder appendCodePoint(int codePoint): This method appends the string representation of the codePoint argument to this sequence.
int capacity(): This method returns the current capacity.
char charAt(int index): This method returns the char value in this sequence at the specified index.
IntStream chars(): This method returns a stream of int zero-extending the char values from this sequence.
int codePointAt(int index): This method returns the character (Unicode code point) at the specified index.
int codePointBefore(int index): This method returns the character (Unicode code point) before the specified index.
int codePointCount(int beginIndex, int endIndex): This method returns the number of Unicode code points in the specified text range of this sequence.
IntStream codePoints(): This method returns a stream of code point values from this sequence.
StringBuilder delete(int start, int end): This method removes the characters in a substring of this sequence.
StringBuilder deleteCharAt(int index): This method removes the char at the specified position in this sequence.
void ensureCapacity(int minimumCapacity): This method ensures that the capacity is at least equal to the specified minimum.
void getChars(int srcBegin, int srcEnd, char[] dst, int dstBegin): This method characters are copied from this sequence into the destination character array dst.
int indexOf(): This method returns the index within this string of the first occurrence of the specified substring.
StringBuilder insert(int offset, boolean b): This method inserts the string representation of the boolean alternate argument into this sequence.
StringBuilder insert(): This method inserts the string representation of the char argument into this sequence.
int lastIndexOf(): This method returns the index within this string of the last occurrence of the specified substring.
int length(): This method returns the length (character count).
int offsetByCodePoints(int index, int codePointOffset): This method returns the index within this sequence that is offset from the given index by codePointOffset code points.
StringBuilder replace(int start, int end, String str): This method replaces the characters in a substring of this sequence with characters in the specified String.
StringBuilder reverse(): This method causes this character sequence to be replaced by the reverse of the sequence.
void setCharAt(int index, char ch): In this method, the character at the specified index is set to ch.
void setLength(int newLength): This method sets the length of the character sequence.
CharSequence subSequence(int start, int end): This method returns a new character sequence that is a subsequence of this sequence.
String substring(): This method returns a new String that contains a subsequence of characters currently contained in this character sequence.
String toString(): This method returns a string representing the data in this sequence.
void trimToSize(): This method attempts to reduce storage used for the character sequence. 
![Capture](https://user-images.githubusercontent.com/99464989/230714031-e0e40ca3-f360-4c2e-b6d5-20d4255a227c.PNG)






![Capture](https://user-images.githubusercontent.com/99464989/230714002-215ba16f-1a8f-4494-9fdc-01e7c04ef8e5.PNG)
![Capture](https://user-images.githubusercontent.com/99464989/230714055-d4f925fd-19cd-42fa-af0f-822ec74f1c0c.PNG)
StringBuilder append() Method in Java With Examples
The java.lang.StringBuilder.append() method is used to append the string representation of some argument to the sequence. There are 13 ways/forms in which the append() method can be used by the passing of various types of arguments:

StringBuilder append(boolean a) :The java.lang.StringBuilder.append(boolean a) is an inbuilt method in Java which is used to append the string representation of the boolean argument to a given sequence.
Syntax :

public StringBuilder append(boolean a)
Parameter: This method accepts a single parameter a of boolean type and refers to the Boolean value to be appended.
Return Value: The method returns a reference to this object.

Examples:

Input: 
string_buffer = "We are Indians" 
boolean a = true

Output: We are Indians true
Below program illustrates the java.lang.StringBuilder.append() method:
![Capture](https://user-images.githubusercontent.com/99464989/230736995-ecf04953-76d1-4bda-a0df-0d69aeb86e1b.PNG
