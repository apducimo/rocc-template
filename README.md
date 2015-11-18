rocc-template
=============

If cloned into rocket-chip directory use

    ./install-symlinks

You can then test it using the emulator

    cd ../emulator && make CONFIG=Sha3CPPConfig run-asm-tests

You can emulate the software implementation of sha3 by running
    ./emulator-Top-Sha3CPPConfig pk ../sha3/tests/sha3-sw.rv +dramsim

or

    ./emulator-Top-Sha3CPPConfig pk ../sha3/tests/sha3-sw-bm.rv +dramsim

You can emulate the accelerated sha3 by running
    ./emulator-Top-Sha3CPPConfig pk ../sha3/tests/sha3-rocc-bm.rv +dramsim

or 

    ./emulator-Top-Sha3CPPConfig pk ../sha3/tests/sha3-rocc.rv +dramsim

The -bm versions of the code omit the print statements and will complete faster.
