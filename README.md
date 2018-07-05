# sscce-ant-compile-trigger

This is a SSCCE for <a href='https://stackoverflow.com/q/51195399/274677'>this SO question</a>.

To highlight the time sensitivity of the Ant [javac] task
invoke the [touch-print-stats-and-invoke-ant-compile] script
in quick succession. E.g if you do:

    ./touch-print-stats-and-invoke-ant-compile && ./touch-print-stats-and-invoke-ant-compile

It is typical that the compilation only happens in the first invocation
but not the second.


NB: For the very first time (or following an 'ant clean') you have
    to invoke 'ant' to create the compiled version of the class.