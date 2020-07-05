# rust-bits

Small examples using the [Rust language](https://www.rust-lang.org) and toolchain.

## Intellij

To use Intellij for development purposes, use this [plugin](https://intellij-rust.github.io).
Follow the included [instructions](https://intellij-rust.github.io/docs/quick-start.html#create-prj) 
to create a new project.

The create folder contents will similar to the one created by `cargo init`, with the addition of the 
Intellij project folder (`.idea`) and file (`.iml`).

## Running

To run the application, do `cargo run` on the shell.
The project can also be ran from inside Intellij.

To build the application, do `cargo build` on the shell.
The application executable will be located inside `target/debug`, because it is a debug build.
It can be ran just by doing `target/debug/rust-bits`.

This last file is already a binary file, as can be seen by doing

```
  rust-bits git:(master) ✗ otool -v -t target/debug/rust-bits |  grep main: -A 4
_main:
00000001000016c0	pushq	%rbp
00000001000016c1	movq	%rsp, %rbp
00000001000016c4	subq	$0x10, %rsp
00000001000016c8	movslq	%edi, %rax
``` 



  
