![Noto](images/noto.png)

# Noto Latin Greek Cyrillic Sources

Source files for generating Noto Latin Greek Cyrillic fonts (Noto Sans, Noto Sans Mono and Noto Serif families)

The files in this repository might be work-in-progress for future versions of the fonts that have not been released yet.
The designs and glyph sets might not final.

## Reporting issues
Issues are currently tracked on the [Google Fonts - Noto Fonts](https://github.com/googlefonts/noto-fonts) repository.
Latin, Greek and Cyrillic issues will be moved here in the future.

## Building

[Python 3.6 or greater](https://www.python.org/downloads/) is required to build the fonts.
To obtain all sources and build tools:

```
$ git clone --recursive https://github.com/notofonts/Noto-LatinGreekCyrillic.git
$ cd Noto-LatinGreekCyrillic
$ ./build setup
```

To build everything from source:

```
$ ./build all
```

other build options exist:

```bash
$ ./build sources/NotoSans-MM.glyphs  # build from a single source
$ ./build variable src/NotoSans-MM.glyphs  # build a single variable font
$ ./build all variable  # build all variable fonts
$ ./build all force
$ ./build all variable force  # continue building even when some sources fail
```

be sure to update this repository and its dependencies on subsequent runs:

```
$ git pull
$ ./build setup
$ ...
```

## License

Noto source (under the `sources` subdirectory) is under the [SIL Open Font License, version 1.1](https://github.com/notofonts/Noto-LatinGreekCyrillic/tree/main/sources/LICENSE).

Build scripts are under the [Apache license, version 2.0](LICENSE).

## Contributing

To contribute to this project, please read [CONTRIBUTING](CONTRIBUTING.md) and [FONT_CONTRIBUTION](FONT_CONTRIBUTION.md)

## News

* 2021-05-17: merged Noto Sans Display into Noto Sans, and Noto Serif Display into Noto Serif  as `opsz` axis.
* 2021-05-10: split Noto Latin Greek Cyrillic from https://github.com/googlefonts/noto-source.

