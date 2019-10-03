hero: Hello, name! demonstration (v0.2.0)

# Remove the software

To remove the software components after completing the demonstration:

1. Stop the nodemanager process first.

    <code style="font-weight:bold;">kill $(pgrep nodemanager)</code>

1. Stop the client process.

    <code style="font-weight:bold;">kill $(pgrep client)</code>

1. Remove all of the SDK files and folders you no longer want to use from your local computer.

    For example, if you downloaded the SDK source code ZIP file, run the following commands:

    <pre style="font-weight:bold;">
    cd ~/Downloads
    rm -rf sdk-0.2.0*
    </pre>