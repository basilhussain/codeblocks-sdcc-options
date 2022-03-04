# Code::Blocks SDCC Compiler Options

This is an updated [SDCC](http://sdcc.sourceforge.net/) compiler options configuration file (`options_sdcc.xml`) for the [Code::Blocks IDE](https://www.codeblocks.org/), improving on the version included in the current (at time of writing) release version of Code::Blocks, 20.03. It has been updated to reflect command line options and features available in the 4.2.0 release of SDCC.

A summary of the changes:

- Reorganised with some new categories: code generation, debugging, warnings.
- Added many new options, removed some old defunct options.
- Added new target CPU architectures: z80n, r2ka, r3ka, mos6502, sm83 (renaming of gbz80).
- Made some newer features conditional on detected SDCC version (e.g.  sm83 vs. gbz80) as not all Code::Blocks users may have latest SDCC version.

## Compatibility

This options file is only compatible with versions of Code::Blocks between release 20.03 and nightly builds older than revision 12739.

**All nightly builds based on revision 12739 or newer already contain the changes from this options file.** If using one of those (or a later release), you do not need this.

Also note that the compiler version-specific conditional presentation of some options only extends back to SDCC version 3.8.0 (circa 2018). It is presumed that SDCC users will not potentially be using versions more ancient than that.

## How to Use

Copy the `options_sdcc.xml` file into the `share\CodeBlocks\compilers` folder inside the Code::Blocks installation folder. You may want to make a copy of (or rename) the original file first. Then restart (or start) Code::Blocks.

## Resources

* [Code::Blocks compiler options file documentation](https://wiki.codeblocks.org/index.php/Compiler_options_file)
* [Code::Blocks compiler definition file documenation](https://wiki.codeblocks.org/index.php/Compiler_file)