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

