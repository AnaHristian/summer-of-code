# Required Homework for Certification
## Day 1
1. Hours in a year. How many hours are in a year? 
2. Minutes in a decade. How many minutes are in a decade? 
3. Your age in seconds. How many seconds old are you? (I'm not going to check your answer, so be as accurate—or not—as you want.)  
4. Andreea Visanoiu: I'm 48618000 seconds old hahaha. Calculate @Andreea Visanoiu's age.
## Day 3
5. Full name greeting: 
  - Write a program that asks for a person’s first name, then middle, and then last. 
  - Finally, it should greet the person using their full name.
6. Bigger, better favorite number:
  - Write a program that asks for a person’s favorite number. 
  - Have your program add 1 to the number, and then suggest the result as a bigger and better favorite number. (Do be tactful about it, though.)
7. Angry Boss: 	
  - Write an angry boss program that rudely asks what you want. 
  - Whatever you answer, the angry boss should yell it back to you and then fire you. 
  - For example, if you type in I want a raise, it should yell back like this: 'WHADDAYA MEAN "I WANT A RAISE"?!? YOU'RE FIRED!!'  
8. Table of Contents:
  - Here’s something for you to do in order to play around more with center, ljust, and rjust: write a program that will display a table of contents (see day3.md to review the format);
## Day 4
9. 99 Bottles of Beer on the Wall:
  - Write a program that prints out the lyrics to that beloved classic, “99 Bottles of Beer on the Wall.”
10. Deaf grandma:
  - Whatever you say to Grandma (whatever you type in), she should respond with this: HUH?! SPEAK UP, GIRL! unless you shout it (type in all capitals). 
  - If you shout, she can hear you (or at least she thinks so) and yells back: NO, NOT SINCE 1938! 
  - To make your program really believable, have Grandma shout a different year each time, maybe any year at random between 1930 and 1950. 
11. Deaf grandma extended:
  - What if Grandma doesn’t want you to leave? When you shout BYE, she could pretend not to hear you. 
  - Change your previous program so that you have to shout BYE three times in a row. 
  - Make sure to test your program: if you shout BYE three times but not in a row, you should still be talking to Grandma.
12. Leap Years:
  - Write a program that asks for a starting year and an ending year and then puts all the leap years between them (and including them, if they are also leap years). 
  - Leap years are years divisible by 4 (like 1984 and 2004). 
  - However, years divisible by 100 are not leap years (such as 1800 and 1900) unless they are also divisible by 400 (such as 1600 and 2000, which were in fact leap years). What a mess!
13. Find something today in your life, that is a calculation. Go for a walk, look around the park, try to count something. Anything! And write a program about it. e.g. number of stairs, steps, windows, leaves estimated in the park, kids, dogs, estimate your books by bookshelf, toiletries, wardrobe.
14. Building and sorting an array: 
  - Write the program that asks us to type as many words as we want (one word per line, continuing until we just press Enter on an empty line) and then repeats the words back to us in alphabetical order. Make sure to test your program thoroughly; for example, does hitting Enter on an empty line always exit your program? Even on the first line? And the second? Hint: There’s a lovely array method that will give you a sorted version of an array: sorted(). Use it!
15. Table of contents:
  - Write a table of contents program here. 
  - Start the program with a list holding all of the information for your table of contents (chapter names, page numbers, and so on).     - Then print out the information from the list in a beautifully formatted table of contents. Use string formatting such as left align, right align, center.
16. Moo:
  - Write a function that prints out "moo" n times.
17. Old-school Roman numerals:
  - Write a method that when passed an integer between 1 and 3000 (or so) returns a string containing the proper old-school Roman numeral. 
  - In other words, old_roman_numeral 4 should return 'IIII'. 
  - Make sure to test your method on a bunch of different numbers. Hint: Use the integer division and modulus methods. 
  - For reference, these are the values of the letters used: I = 1 V = 5 X = 10 L = 50 C = 100 D = 500 M = 1000
18. “Modern” Roman numerals:
  - Eventually, someone thought it would be terribly clever if putting a smaller number before a larger one meant you had to subtract the smaller one. As a result of this development, you must now suffer. Rewrite your previous method to return the new-style Roman numerals so when someone calls roman_numeral 4, it should return 'IV', 90 should be 'XC' etc.

### Optional
## Day 1
1. How many days does it take for a 32-bit system to timeout, if it has a bug with integer overflow? How about a 64-bit system?  
2. Calculate your age accurately based on your birthday: 
  - (maybe use time of day e.g. 8:23am if you know it, use 12:00 noon midday) 
  - you will need Python modules.
## Day 4
3.  Deaf grandma 1:
  - This part is optional and would be much easier if you read the section on Python’s random number generator under the Math Object. 
  - You can’t stop talking to Grandma until you shout BYE. 
  - Hint: Try to think about what parts of your program should happen over and over again. All of those should be in your while loop. Hint: People often ask me, “How can I make random give me a number in a range not starting at zero?” But you don’t need it to. Is there something you could do to the number random returns to you?
