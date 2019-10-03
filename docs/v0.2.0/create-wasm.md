hero: Hello, name! demonstration (v0.2.0)

# Create a WebAssembly canister from ActorScript

1. From the dfx/examples/hello directory, navigate to the source code directory for the Hello, name program:

    <code style="font-weight:bold;">cd app/canisters/hello</code>

1. Review the ActorScript program code defined in the main.as file by running the following command:

    <code style="font-weight:bold;">more main.as</code>

    The command displays the ActorScript source code.

    <pre style="background:transparent">
    actor {
    public func main(name : Text) : async Text {
        return "Hello, " # name # "!";
        };
    };
    </pre>

1. Type q to quit after viewing the ActorScript source code.

1. Return to the examples/hello directory by running the following command:

    <code style="font-weight:bold;">cd ../../..</code>

1. Build an executable WebAssembly module--the canister--from this simple ActorScript program by running the following command:

    <code style="font-weight:bold;">../../result/bin/dfx build</code>

    The command displays output similar to the following:

    <pre style="background:transparent">
    Version v0.2.0 already installed.
    Building hello...
    </pre>

1. Change to the directory created by the build command.

    <code style="font-weight:bold;">cd build/app/canisters/hello</code>

1. Verify the directory contains the WebAssembly and related application files by running the following command:

    <code style="font-weight:bold;">ls -l</code>

    For example, the command returns output similar to the following:

    <pre style="background:transparent">
    total 112
    -rw-r--r--  1 lisagunn  staff     65 Sep  5 12:24 main.did
    -rw-r--r--  1 lisagunn  staff    165 Sep  5 12:24 main.js
    -rw-r--r--  1 lisagunn  staff  45747 Sep  5 12:24 main.wasm
    </pre>

    This directory contains the main.wasm file that indicates the ActorScript was successfully compiled into WebAssembly code that can be deployed on the developer network.