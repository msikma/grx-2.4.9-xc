GRX 2.4.9 (Git copy)
====================

This is a copy of the GRX 2.4.9 library, uploaded to its own repo here
for easy access, e.g. as a submodule for a project using it.

The [GRX library](http://grx.gnu.de/) was written by Csaba Biegl for
[DJGPP](http://www.delorie.com/djgpp/) (a DOS port of GCC). It supports
other, modern platforms as well.

See the original `readme` file for more information.

## Cross-compiling using DJGPP

For cross-compiling using a DJGPP that runs on a Unix-like platform, it's
simply a matter of following the readme and setting the following variables
in `makedefs.grx`:

    # For cross-compiling, specify prefix for tools including the trailing dash
    # (e.g.   i386-mingw32-   for using i386-mingw32-gcc instead of just gcc)
    CROSS_PLATFORM=/usr/local/djgpp/bin/i586-pc-msdosdjgpp-

    # Specify if you want to use Unix tools on DOS-like platforms
    HAVE_UNIX_TOOLS=y

Of course, replace the cross compiling prefix with your own. The one listed
in this example is for [andrewwutw's cross compiling DJGPP](https://github.com/andrewwutw/build-djgpp),
which is a good option for those looking to build DOS programs on modern
systems.

## License

The GRX graphics library is licensed under the [GNU GPL](http://grx.gnu.de/license.html).