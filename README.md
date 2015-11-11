# superfish
esoteric programming language that is borderline useful

an implementation of deadfish, but with many more commands

####old stuff - originally in deadfish

* i - increment current accumulator
* d - decrement current accumulator
* s - square current accumulator
* o - output current accumulator

####new stuff

* dual accumulators
  * p - swap values of accumulators
  * g - increment current accumulator by value of other accumulator
  * h - decrement current accumulator by value of other accumulator
* r - take the root of the current accumulator
* a - swap between numerical output (default) and ASCII output
* n - input a numerical value into the current accumulator
* j - jump to the number character of the other accumulator

####syntax

* list commands one after the other
  * oioopigopgopgopgopgopgopgopgopgopgopgopgo
* j cannot be the first command, nor can it be fed a negative number
  * jnogood
  * dddg
* \n signifies the end of the program
* whitespace is ignored
* other than that, there are no rules

####quirks

you can't manipulate the value of the second accumulator directly, and the only way to change it is to use p
j changes the current place in the program to the value of the second accumulator, so if you were to write

>iissj          o

the program would output

>16

output is handled differently for numbers and letters, there is a newline after every number output, and there is not
for every text output

>iissoo

would output

>16  
>16

while

>aiiiiiiiisiiiiiiiioriisioiiiiiiiooiiioriiiiiiiiiiiiiiiiiiiiiioiiiiriiiiisddoddddddddoiiioddddddoddddddddorddddsdddoriiiii

outputs

>Hello world!  
>

####licensing

who cares
