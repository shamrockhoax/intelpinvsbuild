# intelpinvsbuild
All things pertaining to building Pintools in Visual Studio without using Pin's MyPinTool Project

## Property Sheets
Version: pin-3.7-97619
Compiler: Visual Studio 2017

Property sheets are used to set Visual Studio properties. In this case, the property sheet was made for VS2017 using pin3.7.97619. This should be easily convertable to other versions. 

To use this sheet:

1. Edit the property sheet "<PINDIR></PINDIR" to add the path to the Intel Pin directory.
2. Create a new empty Visual Studio project
3. Under Project Properties->General set the Configuration Type to Dynamic Library (.dll)
4. Under Project Properties->General set the extension to ".dll"
5. Go to the Property Manager tab (or view->Other Window->Property Manager
6. Expand the Project in the property manager window
7. Right click the appropriate build folder (i.e. Debug|Win32)
8. Click Add Existing Property Sheet
9. Go back to the main solution explorer
10. Either create or add the source file that contains your pintool code

The "pintool.prop" file is for x86 builds. Eventually, I'll add an x64 property sheet, but the x86 sheet can easily be modifed to work with x64.
