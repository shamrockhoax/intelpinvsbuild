# intelpinvsbuild
All things pertaining to building Pintools in Visual Studio without using Pin's MyPinTool Project

## Property Sheets
Property sheets are used to set Visual Studio properties. To use this sheet:

1. Create a new empty Visual Studio project
2. Under Project Properties->General set the Configuration Type to Dynamic Library (.dll)
3. Go to the Property Manager tab (or view->Other Window->Property Manager
4. Expand the Project in the property manager window
5. Right click the appropriate build folder (i.e. Debug|Win32)
6. Click Add Existing Property Sheet
7. Go back to the main solution explorer
8. Either create or add the source file that contains your pintool code

The "pintool.prop" file is for x86 builds. Eventually, I'll add an x64 property sheet, but the x86 sheet can be easily modifed to work with x64.
