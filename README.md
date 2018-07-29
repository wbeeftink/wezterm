## TODO

 * [ ] Load key mapping information from terminfo
 * [ ] Look at unicode width and graphemes for cells
 * [ ] ensure that sgr is reset to default on drop
 * [ ] Option to use alt screen when going raw
 * [x] Mouse reporting mode (and restore on drop)
 * [x] Bracketed paste mode (and restore on drop)

## Windows

Testing via Wine:

```
sudo apt install gcc-mingw-w64-x86-64
rustup target add x86_64-pc-windows-gnu
cargo build --target=x86_64-pc-windows-gnu  --example hello
```

Then, from an X session of some kind:

```
wineconsole cmd.exe
```

and from there you can launch the generated .exe files; they are found under `target/x86_64-pc-windows-gnu/debug`


