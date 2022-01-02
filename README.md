Python tools for working with the [_Creatures_](https://creatures.wiki/) series of games

## File types

File types supported:
- SPR images (read+write, including back.spr)
- S16 images (read+write, including back.s16)
- C16 images (read+write)
- BLK images (read+write, macOS big-endian version not supported)
- Creatures 1 COB/RCB files (read only)
- GEN files (read only, version 3 only)

## Command-line Tools

This library also comes with a number of useful tools. Each tool lives under
the `creaturestools/bin/` directory and can be run like `python creaturestools/bin/$toolname.py`.

Some (eventually, all) of the tools are also configured as entry points, which
means you can `pip install` this repository and then use them immediately, e.g.:

```bash
pip install git+https://github.com/openc2e/pycreaturestools/
spritedumper my_sprite.c16
```

Available tools:
- caossyntaxdumper: Parses a caos.syntax file
- creaturescavesdownloader: Downloads files from Creatures Caves
- creaturescavesextractor: Extracts files downloaded from Creatures Caves
- cobdumper: Takes a C1 COB/RCB and writes a CAOS2Cob script and PNG of the thumbnail
- extract_alb2203_sprs: 👀
- gen2json: Parses a GEN file and outputs a JSON representation
- glstdumper: Parses a GLST block
- gno_dumper: Parses genome notes (GNO) files
- new_breed_installer_extract: Extracts files created by Kinnison's New Breed Installer
- parse_2er: Parses 2ER files
- parse_creaturesarchive: Parses CreaturesArchive files (poorly)
- read_aphro: Parses Aphro, AphroBU, Health, and HealthBU files
- read_pefile: Parses resources from Windows executables
- sfcdumper: Parses SFC files
- sfcdumperv2: Parses SFC files
- spritedumper: Takes a sprite (SPR, S16, C16, or BLK) and writes out the frames as PNGs
- szdd_dumper: Decompresses files compressed on old versions of MS-DOS
- translate_voice: Converts a string of text into Creatures sounds
