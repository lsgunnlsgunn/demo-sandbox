hero: Hello, name! demonstration (v0.2.0)

# Download the SDK directory

1. Navigate to the DFINITY SDK release directory and download the Source code (zip) or Source code (`tar.gz`) appropriate for your operating system.

1. Extract the contents of the file you downloaded by double-clicking the compressed archive or by running the appropriate commands. 

    - If you downloaded the **ZIP** file, double-click the file in your default ~/Downloads directory.
    - If you downloaded the **TAR.GZ** file, open a terminal in your default ~/Downloads directory, then run the following command:

    tar -zxvf sdk-0.2.0.tar.gz

1. Open a terminal, if you are not already in a terminal shell, and change to your default ~/Downloads directory.

    <code style="font-weight:bold;">cd ~/Downloads</code>

1. Change to the sdk-v0.2.0 directory by running the following command:

    <code style="font-weight:bold;">cd sdk-0.2.0</code>

1. Verify the contents of the directory by running the following command:

    <code style="font-weight:bold;">ls -l</code>

    The command displays output similar to the following:

    <pre style="background:transparent">
    total 32
    -rw-r--r--@  1 gunn  staff  817 Sep  6 14:03 README.adoc
    drwxr-xr-x@  3 gunn  staff   96 Sep  6 14:03 assets
    drwxr-xr-x@  5 gunn  staff  160 Sep  6 14:03 ci
    -rw-r--r--@  1 gunn  staff  161 Sep  6 14:03 default.nix
    drwxr-xr-x@ 13 gunn  staff  416 Sep 10 10:05 dfx
    -rw-r--r--@  1 gunn  staff  151 Sep  6 14:03 jobset.nix
    drwxr-xr-x@  7 gunn  staff  224 Sep  6 14:03 nix
    -rw-r--r--@  1 gunn  staff  121 Sep  6 14:03 shell.nix
    </pre>