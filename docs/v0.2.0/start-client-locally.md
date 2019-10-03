hero: Hello, name! demonstration (v0.2.0)

# Start the network client locally

1. Change to the examples/hello directory.

    <code style="font-weight:bold;">cd examples/hello</code>

1. Start the DFINITY internet computer network node manager by running the following command:

    <code style="font-weight:bold;">../../result/bin/dfx start</code>

    If you are prompted to allow or deny network connections, click Allow. The command returns output similar to the following then continues to run both processes in the background:

    <pre style="background:transparent">
    Version v0.2.0 installed successfully.
    Starting up the DFINITY node manager...
    DFINITY node manager started...
    Starting /Users/lisagunn/.cache/dfinity/versions/0.2.0/client 
    /Users/lisagunn/.cache/dfinity/versions/0.2.0/nodemanager 
    /Users/lisagunn/.cache/dfinity/versions/0.2.0/client
    </pre>

1. Verify that client and nodemanager are currently running by running the following command:

    <code style="font-weight:bold;">ps</code>

    If successful, the command returns output similar to the following:

    <pre style="background:transparent">
    PID TTY           TIME CMD
    27237 ttys000    0:00.00 /Users/lisagunn/.cache/dfinity/versions/0.2.0/nodemanager /Users/l
    27240 ttys000    0:00.08 /Users/lisagunn/.cache/dfinity/versions/0.2.0/client
    57632 ttys000    0:01.42 -bash
    </pre>