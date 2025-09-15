# Standalone ofwboot

`ofwboot` extracted from the OpenBSD source tree and tweaked to be built under Linux.

# Build

## Checkout

```bash
git clone https://github.com/kakwa/ofwboot-standalone
cd ofwboot-standalone
```

## Dependencies

- `bmake`
- SPARC64 cross toolchain: `gcc-sparc64-linux-gnu` and `binutils-sparc64-linux-gnu`

Example (Debian/Ubuntu):

```bash
sudo apt-get update -y
sudo apt-get install -y bmake gcc-sparc64-linux-gnu binutils-sparc64-linux-gnu
```

## Compilation

From this directory:

```bash
CC=sparc64-linux-gnu-gcc LD=sparc64-linux-gnu-ld bmake

file ofwboot
```

## Clean

```bash
bmake clean
```
