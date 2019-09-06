hero: Hello, World! demonstration (v0.1.0)

# Remove the software

To remove the software components after completing the demonstration:

1. Stop the <code style="background:transparent">nodemanager</code> process first.

    <pre style="font-weight:bold;">
    pkill nodemanager
    </pre>

1. Stop the <code style="background:transparent">dfinity</code> process.

    <pre style="font-weight:bold;">
    pkill dfinity
    </pre>

1. Remove all of the infrastructure folders you no longer want to use from your local computer.

    For example, to remove the infrastructure directories if the full path to your local copy of the <code style="background:transparent">dfinity</code> release directory is <code style="background:transparent">~/dfinity-0.1.0</code>, run the following commands:

    <pre style="font-weight:bold;">
    cd ~
    rm -rf dfinity-0.1.0
    </pre>

1. Remove all of the SDK folders you no longer want to use from your local computer.

    For example, if you downloaded the <code style="background:transparent">dfx</code> executable from the SDK release directory, run the following commands:

    <pre style="font-weight:bold;">
    rm -rf dfinity-sdk-0.1.0-x86_64-*
    rm -rf dfx
    </pre>

    If you also downloaded the SDK source code ZIP file, run the following command:

    <code style="font-weight:bold;">rm -rf sdk-0.1.0</code>

1. Remove Nix files and folders you no longer want to use from your local computer.

    <pre style="font-weight:bold;">
    sudo rm -rf /etc/nix ~/.nix-profile ~/.nix-channels
    </pre>