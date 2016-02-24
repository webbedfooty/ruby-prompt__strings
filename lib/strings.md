---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a sequence of characters, that are, wait for it, strung together; identified by either single or double quotation marks. 

# What are some examples of information that would be Strings as opposed to some other data type?

Anything to be processed simply as text, as opposed to numeric or Boolean values which are evaluated/analyzed.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

A = "Ava Lovelace"
A.byteslice(5)  #=> "o"
A.byteslice(7)  #=> "e"
will return a value of nil if the initial offset falls outside the string

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yes,
A.byteslice(-7)  #=> "v"
it means counting backwards from the end

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

A = "Sumeet Jain"
A.gsub('e','!')


---   Epilogue  ---

   A few notes:
#1	names in Ruby, unless they are names of classes (e.g. String, Num, etc.), should start with lower-case letters. Thus, you should have a = "Ava Lovelace" 

yes absolutely - totally overlooked that but understand the need for them to start with lower-case

#2	The byteslice method is fine, but there's a more terse way to do it. What if you do a[ 7 ]? Does that give you the same thing as a.byteslice(7)?

Yes, you do get the same thing using either method. 
However, with the number set at 7, it actually gives me the 8th character "e";
so I really need to change the number to 5 so I get the 6th character which is "o". 
1st character = position 0 = A 
2nd character = position 1 = v
3rd character = position 2 = a 
4th character = position 3 = _
5th character = position 4 = L 
6th character = position 5 = o  - winner!
7th character = position 6 = v
8th character = position 7 = e 
