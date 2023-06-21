# Advent_of_Code_2022
A C++ 20 Implementation of the Advent of code challenges used to learn the latest features of the cpp sepcification
and to use as many modern features as I can find.

to be clear this is my first advent of code challenge and I am doing and I have not seen any other attempts at this
so please take this for what it is, a completely raw run through of these challenges

## Caviats

As this is a group silly fun challenges i will be developing this with a linux only mindset, if this code does
compile and run on other platforms that is a supprise to me.

These solutions will not be the cleanest most efficent solutions but a good enough for most cases job. while
I do find it intresting to learn from experts on optimsation and ease of reading code. In most cases I 
see what they do as a goal to strive for and not something that should be religously persued. for me fix the
problems you have not the future problems that might occur is my general goal. so will i optomise my code 
not unless running it becomes slow enough to annoy me, will I go over every line with a fine tooth cone
making it as readable as possible. not unless I am struggling to understand it.

## Project structure

I am going to use cmake and ctest for building and testing these application as well as my inline test-utils.hpp 
test framework to run and test these applications.

each day will have its own cmake file that shall act as its indipendent cmake file containing all of the infomation for testing,
and will contain the folders src where the cpp files live inc which contains the hpp files, a read me and a cmake file.
these should be enough to build all of the challeneges

