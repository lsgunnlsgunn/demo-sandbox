hero: Hello, name! demonstration (v0.2.0)

# View command-line usage information

To view usage information for the DFINITY executor (dfx) command-line interface:

1. Check you current working directory by running the following command:

    <code style="font-weight:bold;">pwd</code>

1. If your current directory is dfx/examples/hello, you can view usage information by running the following command:

    <code style="font-weight:bold;">../../result/bin/dfx help</code>

    The command displays information about the flags and subcommands you can use similar to the following:

    <pre style="background:transparent">
    dfx 0.2.0
    The DFINITY Executor.

    USAGE:
        dfx [SUBCOMMAND]

    FLAGS:
        -h, --help       Prints help information.
        -V, --version    Prints version information.

    SUBCOMMANDS:
        build    Builds a specific canister or all canisters. 
        help     Prints this message or the help of the given subcommand(s).
        send     Sends a "Hello World" request to the canister 42.
        start    Start a local network in the background.
    </pre>