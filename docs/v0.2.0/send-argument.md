hero: Hello, name! demonstration (v0.2.0)

# Send an argument to the preconfigured canister

In this demonstration, there is a pre-compiled WebAssembly application deployed in a preconfigured canister that can receive an argument in a user request through the DFINITY SDK command-line interface (dfx) and can return a response that verifies the argument .

To test sending a request with an argument to a precompiled canister:

1. Navigate back to the dfx/examples/hello directory.

    <code style="font-weight:bold;">cd ../../../..</code>

1. Run the following command to simulate sending a your-name argument to a preconfigured canister using the /api/v1/read endpoint to return a response:

    <code style="font-weight:bold;">../../result/bin/dfx send http://localhost:8080 your-name</code>

1. Verify the response returned displays the your-name argument you specified.

    For example, if you specify DFINITY as the argument:

    <pre style="background:transparent">
    Version v0.2.0 already installed.
    Hello, DFINITY!
    </pre>

    Note  If you have previously installed the software and see Hello, World! instead of the argument you specified, you have an outdated version of the client still running on your local computer. If you run into this issue, you can remove the outdated client by running the following command:

    <code style="background:transparent">rm -rf ~/.cache/dfinity</code>

    After removing the cached file, you can re-run the send command to see the argument you specified returned.