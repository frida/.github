Dynamic instrumentation toolkit for developers, reverse-engineers, and security
researchers. Learn more at [frida.re](https://frida.re).

## Where things live

| Organization | What's there |
|---|---|
| [frida](https://github.com/frida) | Frida itself: the runtime, tools, language bindings, and the Luma GUI |
| [frida-packages](https://github.com/frida-packages) | Packages you build on: runtime bridges, agent tooling, Node.js compatibility modules |
| [frida-forks](https://github.com/frida-forks) | Patched forks of third-party projects. Not a list of things Frida needs |
| [frida-labs](https://github.com/frida-labs) | Experiments, demos, and conference material |

## Main repositories

- [frida](https://github.com/frida/frida): releases, and the umbrella repository tying them together
- [frida-gum](https://github.com/frida/frida-gum): instrumentation engine and the GumJS runtime
- [frida-core](https://github.com/frida/frida-core): injection, sessions, and the compiler
- [frida-tools](https://github.com/frida/frida-tools): CLI tools such as `frida`, `frida-trace`, and `frida-pm`
- [luma](https://github.com/frida/luma): the Frida GUI

Language bindings:
[Python](https://github.com/frida/frida-python) ·
[Node.js](https://github.com/frida/frida-node) ·
[Swift](https://github.com/frida/frida-swift) ·
[Go](https://github.com/frida/frida-go) ·
[Rust](https://github.com/frida/frida-rust) ·
[.NET](https://github.com/frida/frida-net) ·
[QML](https://github.com/frida/frida-qml) ·
[Pharo](https://github.com/frida/frida-pharo) ·
[Browser](https://github.com/frida/frida-web-client)

## Building from source

Clone the repository you want and run `make`. Run `./configure` first to pick
options or to cross-compile. Dependencies are fetched through Meson wraps, so a
language binding like [frida-python](https://github.com/frida/frida-python)
pulls in frida-core by itself.

For frida-server, frida-portal, frida-inject, frida-gadget, and the other
binaries, clone [frida-core](https://github.com/frida/frida-core) and run
`make`.

Out-of-tree builds work like autotools: run the repository's `configure` from
the build directory you want. Run from the repository root, it uses `./build`.
