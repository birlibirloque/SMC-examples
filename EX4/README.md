


                         Java Example 4


Simplistic, graphical simulation of a stoplight. Demonstrates
how to use state machines to handle external events (in this case
timeouts).


+ Building
----------

    $ mvn package

+ Reports
---------

    mvn smc:smcreports

(Output in target/site/smc)

+ Executing
-----------

    $ java -jar target/Traffic-jar-with-dependencies.jar

Click on the "Configure..." button and modify the demo's
settings. Increase the vehicle speed and appearance
rate. Decrease the stoplight times.

Also, click on "Pause" and "Continue". "Stop" halts the
demonstration but does not terminate the demo.
