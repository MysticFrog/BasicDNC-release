# BasicDNC

RS232 file transfer between a PC and CNC controls: drip feed, whole-file
upload, receive, and answering a machine's own program requests. Written in
Rust with an egui front end, for Windows.

## Command line

```bash
basic_dnc.exe --machine "Haas VF2" C:\nc\O1234.nc
```

Queues those files for that machine at startup, which is what an Explorer
"Send to" shortcut needs. Files dragged onto the window open the same dialog.

## Dependency licences

`THIRD_PARTY.md` carries the attribution list; regenerate it with
`cargo about`. `deny.toml` holds the allowlist for `cargo deny check licenses`.
