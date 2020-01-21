# intelpinvsbuild
All things pertaining to building Pintools in Visual Studio without using Pin's MyPinTool Project

## Property Sheets
Version: pin-3.7-97619
Compiler: Visual Studio 2017

Property sheets are used to set Visual Studio properties. In this case, the property sheet was made for VS2017 using pin3.7.97619. This should be easily convertable to other versions. 

To use this sheet:

01. Edit the property sheet "<PINDIR></PINDIR" to add the path to the Intel Pin directory.
02. Create a new empty Visual Studio project
03. Go to the project properties
04. Set the "Configuration" drop down to "All Configurations"
05. Set the "Platform" drop down to "All Platforms"
06. On the same Window: Configuration Properties->General set the Configuration Type to Dynamic Library (.dll)
07. On the same Window: Configuration Properties->General set the extension to ".dll"
08. Click "Apply" and "Ok"
09. Go to the Property Manager tab (or view->Other Window->Property Manager
10. Expand the Project in the property manager window
11. Right click the appropriate build folder (i.e. Debug|Win32)
12. Click Add Existing Property Sheet
13. Go back to the main solution explorer
14. Either create or add the source file that contains your pintool code

The "pintool.prop" file is for x86 builds. Eventually, I'll add an x64 property sheet, but the x86 sheet can easily be modifed to work with x64.
