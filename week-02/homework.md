# Required
## Day 1
1. Calculate a table for each letter in the alphabet from a-z, and count how many times each letter appears in alice_in_wonderland.txt (fancy word for counting stuff is "frequency distribution" - because you are counting the frequency of something)
    a: 34,560
    b: 5,027
    ...
    z: 893
    Store the results in a list of lists:

    result = [  
                ["a", 34560], 
                ["b", 5027], 
                ... 
                ["z", 893]
             ]

    - Hint: use python's lower() method to turn all alphabetic letters into small case and count them (so "A" counts towards "a").
    - Hint: Ignore non-alphabetic numbers, you can check with python isalpha() method.
## Day 2
2. Numbers to Letters the chr() method 
  ```
  for letter, frequency in alphabet_table:
    print(letter, frequency)
  ```
There is something small that needs fixing. Can you spot it and fix it? 
  - (Hint, we only want A-Z and a-z) (see day2.md to see the code to fix).  
3. Print char:
  - Make a function that prints A-Z and a-z
4. Cypher:
  - Make a function that asks the user for a message, and turns it into a list of numbers. (It's a cypher ;))
5. 	Write a function that prints out all elements of the above board (world in Civilization III), starting from the first element of the first line, till the end. Each line should be read from beginning to end.
```
M = "land"
o = "water"
world = [
        [o,o,o,o,o,o,o,o,o,o,o],
        [o,o,o,o,M,M,o,o,o,o,o],
        [M,o,o,o,o,o,o,o,M,M,o],
        [o,M,M,M,o,o,o,o,o,M,o],
        [o,o,o,M,o,M,M,o,o,o,o],
        [o,o,o,o,M,M,M,M,o,o,o],
        [o,o,o,M,M,M,M,M,M,M,M],
        [o,o,o,M,M,o,M,M,M,o,o],
        [o,o,o,o,o,o,M,M,o,o,o],
        [o,M,o,o,o,M,o,o,o,o,o],
        [o,o,o,o,o,M,o,o,o,o,o]
        ]
```
6. Now write a function that prints out all elements in reverse.
7. 	Continent Counter Bug:
```
def continent_counter(world, x, y):
    if world[x][y] != "land":
    # Either it's water or we already counted it,​
    # but either way, we don't want to count it now.​
        return 0
    # So first we count this tile...​
    
    size = 1
    world[x][y] = "counted land"

    # ...then we count all of the neighboring eight tiles​
    # (and, of course, their neighbors by way of the recursion).​

    size = size + continent_counter(world, x-1, y-1)
    size = size + continent_counter(world, x  , y-1)
    
    size = size + continent_counter(world, x+1, y-1)
    size = size + continent_counter(world, x-1, y)
    size = size + continent_counter(world, x+1, y)
    size = size + continent_counter(world, x-1, y+1)

    size = size + continent_counter(world, x, y+1)
    size = size + continent_counter(world, x+1, y+1)    
    return size

print(continent_counter(world, 5, 5))
```
  - There is one small bug in the continent counter above. Can you find it and fix it? 
  - Hint: change the world so that the continent borders the edge.
8. Continent Counter n x n:
  - Write a function that generates an n x n sized board with either land or water chosen randomly.
## Day 3
9. Modify "a" for another name in my_dict. Hint: you will have to create a new key-value pair, copy in the value, and then delete the old one.
10. Redo the frequency distribution of alice_in_wonderland.txt and save your result in a dictionary
```
Store the results in a dictionary:

result = {  
            "a", 34560, 
            "b", 5027, 
            ... 
            "z", 893
         }
 ```
11. Create a dictionary with your own personal details, feel free to be creative and funny so for example, you could include key-value pairs with quirky fact, fav quote, pet. Practice adding, modifying, accesing.
12. Review the chat reply of today's beautiful class interaction and instantiate a student variable for everyone who shared their dream.
13. Translate the real world 1MWTT student into a Student class, decide on all the attributes that would be meaningful. 
  - Hint: You can start with the DIY signup form https://memberportal.1millionwomentotech.com/diy but feel free to be creative and add/modify as you see it best! 
  - This is the REAL work of a creator to find the meaningful description of reality and translate it for computers.

  
# Optional
## Day 1
1. If you have already started Python the Hard Way, please choose 5 exercises and write tests for those in unittest and make them pass.
## Day 2
2. Ceaser cypher: Write a function that does a ceaser cypher (Google), ask the user a number, and shift their message by that number.
3. Run your continent counter for a 20 x 20 board. How long does it take to run? (If it runs quickly, try 30 x 30 ... 100 x 100 just be aware you might end up in a VERY LOOOONG WAIT) - make sure you know how to break a running program as it may take a long time to complete and you might not have time to wait for it ;)
Write test coverage in unittest and/or trace for Continent Counter.
## Day 3
4. Mapping with cities and states/regions in your country or some other country. Find the Python documentation for dictionaries and try to do even more things to them. Find out what you can't do with dictionaries. A big one is that they do not have order, so try playing with that.
5. test to check the outcome of the alice_in_wonderfland, List of Lists
6. test to check the outcome of the alice_in_wonderfland, Dict
7. Come up with a whole taxonomy of Classes for 1MWTT: Person() => Student(), Mentor(), Volunteer(), Employer(). Feel free to suggest/invent and also use mixins, decorators, and any other design patterns that you see would help reach the mission of 1 million women to tech by 2020.
8. Write some more songs using this and make sure you understand that you're passing a list of strings as the lyrics. Put the lyrics in a separate variable, then pass that variable to the class to use instead. See if you can hack on this and make it do more things. Don't worry if you have no idea how, just give it a try, see what happens. Break it, trash it, thrash it, you can't hurt it.
9. Search online for "object-oriented programming" and try to overflow your brain with what you read. Don't worry if it makes absolutely no sense to you. Half of that stuff makes no sense to me too.
## Day 4:
10. http://jfine-python-classes.readthedocs.io/en/latest/subclass-int.html
