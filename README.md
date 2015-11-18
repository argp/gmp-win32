# gmp-win32 - a Win32 port of GMP

## Introduction 

This is a collection of the files that I modified in order to get the
GNU Multiple Precision Arithmetic Library (GMP) version 3.1.1 to compile
on Windows 32.  Please note that this port has no dependencies on third
party software.  Also, I have only tested it on a Windows XP machine with
MS Visual Studio .NET 2003.

## Compilation and installation

To compile it just copy the files provided here to the distribution
directory of GMP 3.1.1 and overwrite the existing files there, then simply
enter the directory and type nmake.  If you don't use MS VS .NET 2003 you
would have to change the related include line in the Makefile.  There is no
installation required, just put gmp.h to your include path and gmp.lib to
your library path.  When you are using it in MSVC++ to compile new programs
don't forget to define _NTRG_WIN32_, include gmp.h and link against gmp.lib.

In the directory bin/ you can find a pre-compiled version.
