# musl-cross

This is a simple, lightweight project for making cross-compilation toolchain with musl libc.

## Supported targets

| Target                         | Kernel  | Binutils | GCC    | Musl  | mold   |
|--------------------------------|---------|----------|--------|-------|--------|
| aarch64-unknown-linux-musl     | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 | 2.40.4 |
| arm-unknown-linux-musleabi     | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| arm-unknown-linux-musleabihf   | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| armv7-unknown-linux-musleabi   | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| armv7-unknown-linux-musleabihf | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| i586-unknown-linux-musl        | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| i686-unknown-linux-musl        | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| loongarch64-unknown-linux-musl | 5.19.16 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| m68k-unknown-linux-musl        | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| microblazeel-xilinx-linux-musl | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| microblaze-xilinx-linux-musl   | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| mipsel-unknown-linux-musl      | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| mipsel-unknown-linux-muslsf    | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| mips-unknown-linux-musl        | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| mips-unknown-linux-muslsf      | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| mips64el-unknown-linux-musl    | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| mips64-unknown-linux-musl      | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| powerpc-unknown-linux-musl     | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| powerpc64-unknown-linux-musl   | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| riscv32-unknown-linux-musl     | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| riscv64-unknown-linux-musl     | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| s390x-ibm-linux-musl           | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| sh4-multilib-linux-musl        | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |
| x86_64-unknown-linux-musl      | 5.4.302 | 2.46.0   | 15.2.0 | 1.2.6 |        |

## How to use

Download the tarball from the [release page](https://github.com/cross-tools/musl-cross/releases) and extract it to `/opt/x-tools`:

```sh
sudo mkdir -p /opt/x-tools
sudo tar -xf ${target}.tar.xz -C /opt/x-tools
```

## How to build

Fork this project and create a new release, or build manually:

```sh
./scripts/make ${target}
```

## License

MIT

## Acknowledgements

We would like to express our gratitude to the following individuals and projects:

- [crosstool-ng](https://github.com/crosstool-ng/crosstool-ng)
- [musl-libc](https://musl.libc.org)
