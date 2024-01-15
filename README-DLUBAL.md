This branch has been customized to be easier to build for RFEM/RSTAB.

#### Build instructions:

1. initialize git submodules using git submodule update
2. open the Visual Studio 2019 command line in the ./win directory
3. run `build-deps.cmd` for both Debug and Release:
	`build-deps.cmd vs2017-x64 Debug`
	`build-deps.cmd vs2017-x64 Release`
4. set variables with paths to OpenCascade headers and libraries, e.g.:
	`set OCC_INCLUDE_DIR=d:\Sources\R20_2\src\3rdParty\OCE\include\oce\`
	`set OCC_LIBRARY_DIR=d:\Sources\R20_2\lib_win64_msvc\debug\`
5. run `run-cmake.bat`
6. build the generated solution with Visual Studio