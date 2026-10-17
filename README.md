# telnet

Telnet for [polpo](https://github.com/polpo-system/polpo): a telnet client in a viewer of the
desktop, a VT100 terminal (the package terminals) over a connection of NetSystem.

```
portia.Install telnet
```

## Using

    Telnet.Open host [port]     a connection in a new viewer (port 23 if none is given)
    Telnet.Close                (in its menu) ends the connection
    Telnet.Send text            sends text to the marked terminal
    Telnet.OpenLog              a viewer with what was received

## What is here

    src/Telnet.Mod        the client
    tools/Telnet.Tool
    test/TelnetTest.Mod

The source comes from ETH Linux Oberon (OLR, 2017-06-18), converted from an Oberon text to plain
text; the first commit has it unchanged. It compiles unchanged with all five of polpo's compilers
(x86, ARM, ARMv7, RISC-V, MIPS).

## Tests

    TelnetTest.Run      1 check: the module loaded; it needs the desktop's display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
