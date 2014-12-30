


                         Java Example 2


This state machine "recognizes" the string 0*1*. Example 2 differs
from example 1 in that example 2 uses default transitions.


+ Building
----------

    mvn package

+ Reports
---------

    mvn smc:smcreports

(Output in target/site/smc)

+ Executing
-----------

    $ java -jar target/checkstring-jar-with-dependencies.jar <string>

Try several different strings, such as:

    $ java -jar target/checkstring-jar-with-dependencies.jar ""
      -> acceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar 000
      -> acceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar 00011
      -> acceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar 111
      -> acceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar 000111100
      -> unacceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar 00011a1b10c0
      -> unacceptable
