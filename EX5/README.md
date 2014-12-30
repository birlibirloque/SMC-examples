


                         Java Example 5


Simplistic, graphical simulation of a task processing.
Demonstrates state Entry actions.


+ Building
----------

    $ mvn package

+ Reports
---------

    mvn smc:smcreports

(Output in target/site/smc)

+ Executing
-----------

Unix & Windows:

    $ java -jar target/taskdemo-jar-with-dependencies.jar

Click on "Create Task..." button and start a new task
running. If you want to create multiple tasks, click the
"Apply" button rather than "OK" since "OK" causes the
dialog box to be removed.

After creating one or more tasks, go to the task table and
click on a task row. Notice select an item from the pop-up
menu.

Also change the log message display to increase or decrease
message detail (the greater the level, the greater the
detail).
