# libarchive for RACE

This repo provides scripts to custom-build the
[libarchive library](https://github.com/libarchive/libarchive) for RACE.

## License

The libarchive library is licensed under the 2-Clause BSD license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

libarchive has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build libarchive.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-libarchive.git
./ext-builder/build.py \
    --target android-x86_64 \
    ./ext-libarchive
```

## Platforms

libarchive is built for the following platforms:

* `android-x86_64`
* `android-arm64-v8a`

It is also used on Linux but can be installed via `apt`.

## How It Is Used

libarchive is used directly by the RACE core.
