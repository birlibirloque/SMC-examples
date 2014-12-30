


                         Java Example 3


This state machine "recognizes" the palindromes (words that read the
same backwards as forwards). The words consist of the alphabet
{0, 1, c} where the letter 'c' may appear only once and marks the
words center.


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
      -> unacceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar 00
      -> unacceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar 1c
      -> unacceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar c0
      -> unacceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar abcba
      -> unacceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar 110010c010011
      -> acceptable
    $ java -jar target/checkstring-jar-with-dependencies.jar 110010c110010
      -> unacceptable
