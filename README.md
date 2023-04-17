# jOSh-nexus-tsiraM

This repository contains a culmination of my work over 3 semesters in Computer Organization and Architecture, Operating Systems, and Design of Compilers. tsiraM is a virtual 6502 CPU written in TypeScript that is able to execute a subset of the original 6502 instruction set. jOSh is an operating system written in TypeScript that runs on top of tsiraM and manages the execution of many programs as well as a virtual file system. Lastly, Nexus is a compiler for a custom language grammar written in Rust but compiled into WebAssembly so it can run in the browser. Nexus supports a subset of the tsiraM instruction set as well as RISC-V assembly for the target outputs and is able to send the 6502 output directly to jOSh to be loaded and executed.

## Setup Instructions
1. Install Node.js, which can be found [here](https://nodejs.org/en).
2. Install Rust, which can be found [here](https://www.rust-lang.org/tools/install).
3. Make sure Node.js and Rust are in your $PATH. Default locations are *~/.npm-global/bin* and *~/.cargo/bin*, respectively.
4. Install TypeScript by running the command `npm i -g typescript`.
5. Install wasm-pack by running the command `cargo install wasm-pack`.
6. *Recommended:* Install serve by running the command `npm i -g serve`.

## Compilation and Startup Instructions
1. Compile tsiraM and jOSh by running `tsc` from the project's root directory.
2. Compile Nexus by running `make`/`make build` from the project's root directory.
3. Spin up a web server by running `make run` from the project's root directory.
4. Open up a modern and updated web browser (Firefox and Chrome are recommended) to *localhost:3000* (or whatever port the server is running on in case port 3000 is already in use).

## More Information
* [jOSh](https://github.com/joshuaseligman/jOSh)
* [Nexus](https://github.com/joshuaseligman/nexus-compiler)
