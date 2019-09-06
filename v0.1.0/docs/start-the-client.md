hero: Hello, World! demonstration (v0.1.0)

# Start the client process

1. Start the DFINITY internet computer network node manager in the background by running the following command:

    <code style="font-weight:bold;">./result/bin/nodemanager ./result/bin/dfinity &</code>

    If you are prompted to allow or deny network connections, click **Allow**. If successful, the command returns output similar to the following then continues to run both processes in the background:

    <pre style="background:transparent">
    [1] 63541
    Starting ./result/bin/dfinity ./result/bin/nodemanager ./result/bin/dfinity
    </pre>

    Because <code style="background:transparent">nodemanager</code> and <code style="background:transparent">dfinity</code> run as background processes, you can continue working in the same terminal window.

1. Verify that <code style="background:transparent">dfinity</code> and <code style="background:transparent">nodemanager</code> are currently running by running the following command:

    <code style="font-weight:bold;">ps</code>

    If successful, the command returns output similar to the following:

    <pre style="background:transparent">
      PID TTY           TIME CMD
    54336 ttys000    0:00.54 -bash
    63541 ttys000    0:00.01 ./result/bin/nodemanager ./result/bin/dfinity
    63545 ttys000    0:00.06 ./result/bin/dfinity
    </pre>

1. Attempt to stop the DFINITY internet computer network by running the `kill -9` command to force processes to terminate.

    <code style="font-weight:bold;">pkill -9 dfinity</code>

1. Verify that the network node manager automatically restarts the network node:

    <pre style="background:transparent">
    Stopped
    Starting ./result/bin/dfinity ./result/bin/nodemanager ./result/bin/dfinity
    </pre>

1. Re-run the <code style="background:transparent">ps</code> command to verify that <code style="background:transparent">nodemanager</code> restarted the <code style="background:transparent">dfinity</code> process by checking the <code style="background:transparent">dfinity</code> process identifier (PID).

    <code style="font-weight:bold;">ps</code>

    The command returns output similar to the following:

    <pre style="background:transparent">
    PID TTY           TIME CMD
    57632 ttys000    0:00.58 -bash
    63541 ttys000    0:00.01 ./result/bin/nodemanager ./result/bin/dfinity
    63549 ttys000    0:00.02 ./result/bin/dfinity
    </pre>

    The process identifier for <code style="background:transparent">nodemanager</code> remains the same (for example, <code style="background:transparent">63541</code>) because that process continued to run to ensure the availability of the <code style="background:transparent">dfinity</code> process, but the <code style="background:transparent">dfinity</code> process itself has a new process identifier because after the process is terminated by the <code style="background:transparent">kill</code> command, <code style="background:transparent">nodemanager</code> restarts it as a new process.