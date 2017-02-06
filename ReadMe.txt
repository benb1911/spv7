/// ///////////////////////////////:
DIRECTORY
/// ///////////////////////////////:
-Data: all data for test.
-ExternalLib: libraries need for compil source code.
-Gcc: a windows gcc for compil the source code (compatible with theard use in the library).
-Src: source code of the library.
-Test: Example and test function of the library. For windows, use clean.bat to clean all example and test.

/// ///////////////////////////////:
TO COMPILE THE LIBRARY
/// ///////////////////////////////:
*** Pthread:
	Define USE_POSIX_THREAD
	- with mingw-win64 for WIN32 binary:
		- Search directories:
			Compiler and Linker:
				../../ExternalLib/PThread/include
			Linker:
				../../ExternalLib/PThread/lib/x86
		- Linker settings :
			pthreadGC2
	- with TDM-mingw for WIN64 binary:
		- all is included to TDM-mingw or mingw 64bit.

/// ///////////////////////////////:
INSTALL AND USE LIBRARY WITH WIN 7 64bit and mingw 64bit
/// ///////////////////////////////:
1) Install msys2
2) Install mingw 64bit with msys2:
	pacman -S mingw-w64-x86_64-toolchain
	pacman -S make
3) Move make.exe to bin of mingw64.
4) Configure C::B or other IDE to use mingw-w64.	

